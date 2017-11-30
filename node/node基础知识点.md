## node
node是事件驱动，异步执行的JavaScript执行环境

## 异步编程（难点）
  回调函数实现 没有阻塞从而提高性能，可以处理大量的并发请求

## 事件驱动（特别特别重要）
  1 几个重要概念
     事件队列： IO设备完成一个任务，就对向事件队列中添加一个事件，而实践队列相当于一个等待被执行的事件栈
     事件循环： 线程不断循环的去检测事件队列
     事件驱动： 编程主要思想是通过事件或状态的变化来进行应用程序的流程控制，一般通过事件监听完成，
     一旦事件被检测到，则调用相应的回调函数
  2  EventEmitter(事件监听与事件触发的封装）

## buffer
buffer类专门存放而精致数据的缓存区  提供了处理二进制能力


## Stream（难点）
  流是对输入输出设备的抽象接口[参考](https://www.cnblogs.com/dolphinX/p/6285240.html)
 1  流类型
 2  所有流对象都是EventEmitter的实例
 3  流对象的常用事件
 
 ## 模块系统（重点）
 1  require() 加载模块机制
 2  模块的接口  require  export
 
 
 ## 全局对象Global
 1 常见全局变量：__filename __dirname setTimeout() setInterval() console 
 2  process(提供了当前node进程状态信息） 
 
 
 ## 核心及常用模块
  1 fs（文件管理系统）
  2 os(提供操作系统信息）
  3 URL(处理请求url)
  4 Query Strings(处理 get/post 请求传递过来的参数）
  5 Path(处理文件路径）
    
  
