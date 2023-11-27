# Cuda
## Linux安装
1. 准备显卡驱动和Cuda：NVIDIA-Linux-x86_64-515.65.01.run，cuda_11.4.0_470.42.01_linux.run
1. ./NVIDIA-Linux-x86_64-515.65.01.run。遇到错误看'/var/log/nvidia-installer.log'。安装时需关闭XWindow，可以看log里冲突的进程号并kill
1. ./cuda_11.4.0_470.42.01_linux.run。取消选中 Driver安装，用上一步安装的驱动
1. nvcc -V // 确认已安装成功，如命令不存在可把“/usr/local/cuda-11.4/bin/”放到环境path
