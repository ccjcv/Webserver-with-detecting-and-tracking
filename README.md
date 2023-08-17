# Webserver-with-detecting-and-tracking

项目描述：在Linux环境下，使用C++11搭建的Web服务器，经过压力测试后能够实现近一万的并发连接。用户注册后登录网站，能够访问服务器的图片、视频等资源。同时实现了一个基于跳表的KV存储引擎，能够实现数据的增删改查、展示等功能。最后配置了改进扩散模型的检测和追踪显示页面。

主要工作：

1.利用IO复用技术Epoll与线程池实现多线程的Reactor高并发模型。  
2.利用正则与状态机解析HTTP请求报文，实现处理静态资源的请求。  
3.利用标准库容器封装char，实现自动增长的缓冲区。  
4.基于小根堆实现的定时器，关闭超时的非活动连接。  
5.利用单例模式与阻塞队列实现异步的日志系统，记录服务器运行状态。  
6.利用RAII机制实现了数据库连接池，减少数据库连接建立与关闭的开销，同时实现了用户注册登录功能。  
7.通过KV存储引擎实现了数据的增删改查、打印展示、数据落盘和文件加载数据等功能。  
8.改进扩散检测模型的超声肝脏图像、视频检测和追踪的显示（基于改进DiffusionDet的超声肝脏检测、追踪方法及系统）。  

检测界面：
![image](https://github.com/ccjcv/Webserver-with-detecting-and-tracking/blob/main/Screenshot%202023-04-24%20at%2021-43-10%20%E5%8C%BB%E5%AD%A6%E8%B6%85%E5%A3%B0%E5%BD%B1%E5%83%8F%E5%A4%84%E7%90%86.png)

追踪界面：
![image](https://github.com/ccjcv/Webserver-with-detecting-and-tracking/blob/main/Screenshot%202023-04-24%20at%2021-48-17%20%E5%8C%BB%E5%AD%A6%E8%B6%85%E5%A3%B0%E5%BD%B1%E5%83%8F%E5%A4%84%E7%90%86.png)

