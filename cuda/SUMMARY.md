# CUDA
1. **CUDA的快速入门**  
   - [CUDA极简入门](https://zhuanlan.zhihu.com/p/34587739)
   - [CUDA编程接口官方文档](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#programming-interface)
   - [编程手册系列文章](https://zhuanlan.zhihu.com/p/501210131)
   - [CUDA执行模型及GPU架构](https://blog.csdn.net/qq_42683011/article/details/113593860)
1. **CUDA并行编程快速上手**  
   - [并行编程下的矩阵加法](https://zhuanlan.zhihu.com/p/97192227)
   - [并行编程之矩阵乘法](https://blog.csdn.net/sunmc1204953974/article/details/51098028)
1. **并行编程及优化**  
   - [矩阵乘法优化指南](https://zhuanlan.zhihu.com/p/410278370)
   - [GPU软硬件组织结构](https://zhuanlan.zhihu.com/p/97131966)
   - [共享存储程序优化](https://zhuanlan.zhihu.com/p/538351377)
1. **CUDA程序性能分析工具**  
   - [Nsight-系列](https://zhuanlan.zhihu.com/p/132582159)
   - [GPU端的CUDA Event计时](https://zhuanlan.zhihu.com/p/339960063)

## 知识
### 异步
* CUDA流通过任务队列和调度器机制实现异步执行。任务被添加到流的任务队列中，并由调度器在 GPU 上调度执行。使用异步 API 可以立即返回而不阻塞 CPU 线程，从而实现更高效的并行计算和资源利用。

### GPU的多实例（multi-instance）
> 允许在同一个 GPU 上运行多个模型实例，从而提高 GPU 的利用率和吞吐量。

* Triton配置模型的实例组（instance group）的count值
* TensorRT创建多个执行上下文（engine->createExecutionContext()）来实现多实例化，每个执行上下文可以独立地执行推理操作。