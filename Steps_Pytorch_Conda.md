# python:

```bash
py -m ensurepip --upgrade
python -m pip install --upgrade pip

#uninstall:
pip freeze >un.txt
pip uninstall -r un.txt -y
```

# CUDA


installation

  https://docs.nvidia.com/cuda/archive/
  
  CUDA Toolkit and Minimum Required Driver Version for CUDA Minor Version Compatibility:
  
  https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html
  
  https://developer.nvidia.com/cuda-12-6-0-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local


CUDA Verification:

```bash
PS C:\Users\Administrator> nvcc --version
  nvcc: NVIDIA (R) Cuda compiler driver
  Copyright (c) 2005-2024 NVIDIA Corporation
  Built on Fri_Jun_14_16:44:19_Pacific_Daylight_Time_2024
  Cuda compilation tools, release 12.6, V12.6.20
  Build cuda_12.6.r12.6/compiler.34431801_0

PS C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.6\extras\demo_suite> .\bandwidthTest.exe
  [CUDA Bandwidth Test] - Starting...
  Running on...
  
  Device 0: NVIDIA GeForce RTX 4090
  Quick Mode
  
  Host to Device Bandwidth, 1 Device(s)
  PINNED Memory Transfers
  Transfer Size (Bytes)        Bandwidth(MB/s)
  33554432                     18265.0
  
  Device to Host Bandwidth, 1 Device(s)
  PINNED Memory Transfers
  Transfer Size (Bytes)        Bandwidth(MB/s)
  33554432                     17224.6
  
  Device to Device Bandwidth, 1 Device(s)
  PINNED Memory Transfers
  Transfer Size (Bytes)        Bandwidth(MB/s)
  33554432                     737406.8
  
  Result = PASS
  
  NOTE: The CUDA Samples are not meant for performance measurements. Results may vary when GPU Boost is enabled.

PS C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.6\extras\demo_suite> .\deviceQuery.exe
C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.6\extras\demo_suite\deviceQuery.exe Starting...
  
  CUDA Device Query (Runtime API) version (CUDART static linking)
  
  Detected 1 CUDA Capable device(s)
  
  Device 0: "NVIDIA GeForce RTX 4090"
  CUDA Driver Version / Runtime Version          12.6 / 12.6
  CUDA Capability Major/Minor version number:    8.9
  Total amount of global memory:                 23028 MBytes (24146083840 bytes)
  MapSMtoCores for SM 8.9 is undefined.  Default to use 128 Cores/SM
  MapSMtoCores for SM 8.9 is undefined.  Default to use 128 Cores/SM
  (128) Multiprocessors, (128) CUDA Cores/MP:     16384 CUDA Cores
  GPU Max Clock rate:                            2535 MHz (2.54 GHz)
  Memory Clock rate:                             10501 Mhz
  Memory Bus Width:                              384-bit
  L2 Cache Size:                                 75497472 bytes
  Maximum Texture Dimension Size (x,y,z)         1D=(131072), 2D=(131072, 65536), 3D=(16384, 16384, 16384)
  Maximum Layered 1D Texture Size, (num) layers  1D=(32768), 2048 layers
  Maximum Layered 2D Texture Size, (num) layers  2D=(32768, 32768), 2048 layers
  Total amount of constant memory:               zu bytes
  Total amount of shared memory per block:       zu bytes
  Total number of registers available per block: 65536
  Warp size:                                     32
  Maximum number of threads per multiprocessor:  1536
  Maximum number of threads per block:           1024
  Max dimension size of a thread block (x,y,z): (1024, 1024, 64)
  Max dimension size of a grid size    (x,y,z): (2147483647, 65535, 65535)
  Maximum memory pitch:                          zu bytes
  Texture alignment:                             zu bytes
  Concurrent copy and kernel execution:          Yes with 1 copy engine(s)
  Run time limit on kernels:                     Yes
  Integrated GPU sharing Host Memory:            No
  Support host page-locked memory mapping:       Yes
  Alignment requirement for Surfaces:            Yes
  Device has ECC support:                        Enabled
  CUDA Device Driver Mode (TCC or WDDM):         WDDM (Windows Display Driver Model)
  Device supports Unified Addressing (UVA):      Yes
  Device supports Compute Preemption:            Yes
  Supports Cooperative Kernel Launch:            Yes
  Supports MultiDevice Co-op Kernel Launch:      No
  Device PCI Domain ID / Bus ID / location ID:   0 / 43 / 0
  Compute Mode:
  < Default (multiple host threads can use ::cudaSetDevice() with device simultaneously) >
  
  deviceQuery, CUDA Driver = CUDART, CUDA Driver Version = 12.6, CUDA Runtime Version = 12.6, NumDevs = 1, Device0 = NVIDIA GeForce RTX 4090
  Result = PASS
```


# Pytorch:
https://pytorch.org/get-started/previous-versions/

```bash
pip install torch==2.0.0 torchvision==0.15.1 torchaudio==2.0.1 --index-url https://download.pytorch.org/whl/cu118

pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu121

pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```


# Conda:

#创建conda环境（Lion）, python版本（3.9）
#create conda envirionment (named:Lion), python version 3.9

```bash
conda create -n Lion python=3.9
```

#进入conda环境（Lion）
#login conda envirionment (Lion)

```bash
conda activate Lion
```

#退出当前conda环境
#quit conda envirionment (Lion)

```bash
conda deactivate
```

#查看已经建立的conda环境
#check the conda envirionments built

```bash
conda info --envs
```

#删除conda环境（Lion）
#remove the conda envirionment Lion

```bash
conda remove -n Lion --all
```
