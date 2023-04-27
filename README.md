# Webserver-with-detecting-and-tracking

线程池 + 非阻塞socket + epoll(ET和LT均实现) + 事件处理(Reactor和模拟Proactor均实现) 的并发模型。
状态机解析HTTP请求报文，支持解析GET和POST请求。
服务器数据库实现web端用户注册、登录功能，可以请求服务器图片和视频文件。
配置基于pytorch扩散模型检测的目标跟踪网络和Transformer分割网络，进行视频、图像的接收和推理。
