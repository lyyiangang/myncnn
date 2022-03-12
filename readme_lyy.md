# build
```
./run-docker.sh

source env.bashrc

cd build
cmake -DCMAKE_BUILD_TYPE=Release -DNCNN_VULKAN=OFF -DNCNN_SYSTEM_GLSLANG=OFF -DNCNN_BUILD_EXAMPLES=ON ..
make -j3
```

# run example
```bash
cd ../examples
../build/examples/squeezenet ../images/256-ncnn.png

```

# benchmark 
```
cd ../benchmark
../build/benchmark/benchncnn 10 $(nproc) 0 0
```
