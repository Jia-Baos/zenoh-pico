# build 指令

```BASH
mkdir build && cd build

cmake .. \
  -DBUILD_SHARED_LIBS=ON \
  -DBUILD_EXAMPLES=ON \
  -DBUILD_TOOLS=ON \
  -DBUILD_TESTING=ON \
  -DBUILD_INTEGRATION=ON \
  -DCMAKE_INSTALL_PREFIX="$(pwd)/../install-prefix"

cmake --build . --config Release

cmake --install . # or make install

export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/jia-baos/Project-Cpp/zenoh-pico/install-prefix/lib
```
