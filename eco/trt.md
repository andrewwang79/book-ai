# 性能
1. 多线程：每个线程是1个IExecutionContext，会复用模型内存
1. 多batch：1个nvinfer1::IExecutionContext支持多batch，一次输入数据是多个数据(比如1批次是4个数据)