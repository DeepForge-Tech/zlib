# ZLIB - data compression library
## Build
~~~bash
cd zlib
mkdir build
cd build
# static library
cmake .. -DBUILD_SHARED_LIBS=YES # or cmake ..

# shared library
cmake .. -DBUILD_SHARED_LIBS=YES

cmake --build .
~~~
#### ⚙️ [Algorithm](./algorithm.md)
#### 📄 [LICENSE](./LICENSE)
