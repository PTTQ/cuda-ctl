# cuda-ctl
A CUDA forwarding library that can limit resources, adapted from tkestack/vcuda-controller, supports CUDA 11.2.

## Running

Switch to the project root directory.

### Make dynamic link library
```
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make
```

### Copy the dynamic link library to the specified directory
```
cp libcuda-control.so /etc/kube-gpu/vdriver/nvidia/lib64/
cp libcuda-control.so /etc/kube-gpu/vdriver/nvidia/lib64/libcuda.so
cp libcuda-control.so /etc/kube-gpu/vdriver/nvidia/lib64/libcuda.so.1
```
