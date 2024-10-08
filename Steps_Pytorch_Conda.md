# python:

```bash
py -m ensurepip --upgrade
python -m pip install --upgrade pip

#uninstall:
pip freeze >un.txt
pip uninstall -r un.txt -y
```

# CUDA
https://docs.nvidia.com/cuda/archive/

CUDA Toolkit and Minimum Required Driver Version for CUDA Minor Version Compatibility:

https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html


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
