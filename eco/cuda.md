# Cuda
## Linux安装
### 显卡驱动
1. 准备显卡驱动NVIDIA-Linux-x86_64-515.65.01.run
1. apt install gcc make
1. ./NVIDIA-Linux-x86_64-515.65.01.run。遇到错误看'/var/log/nvidia-installer.log'。安装时需关闭XWindow，可以看log里冲突的进程号并kill
1. nvidia-smi // 检查版本是"515.65.01"

### CUDA
1. 准备cuda_11.4.0_470.42.01_linux.run
1. ./cuda_11.4.0_470.42.01_linux.run。取消选中 Driver安装，用上一步安装的驱动
1. nvcc -V // 确认已安装成功，如命令不存在可把“/usr/local/cuda-11.4/bin/”放到环境path

## 知识
### 异步
* CUDA流通过任务队列和调度器机制实现异步执行。任务被添加到流的任务队列中，并由调度器在 GPU 上调度执行。使用异步 API 可以立即返回而不阻塞 CPU 线程，从而实现更高效的并行计算和资源利用。

### GPU的多实例（multi-instance）
> 允许在同一个 GPU 上运行多个模型实例，从而提高 GPU 的利用率和吞吐量。

* Triton配置模型的实例组（instance group）的count值
* TensorRT创建多个执行上下文（engine->createExecutionContext()）来实现多实例化，每个执行上下文可以独立地执行推理操作。