# pixar_rt

follow along with [Postcard Pathtracer](https://fabiensanglard.net/postcard_pathtracer/)

## macos build

```
clang -o card -O3 raytracer.cpp
time ./card > pixar.ppm
```

## windows build

```
git clone https://github.com/InterruptSpeed/pixar_rt
cd pixar_rt
mkdir build64
cd build64
cmake -G "Visual Studio 15 2017 Win64" ..
cmake --build . --config Release
cd Release
pixar_rt.exe > pixar.ppm
```
