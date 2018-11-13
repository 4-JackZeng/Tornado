<center>torando</center>

####torando的应用场景：

* 1 用户量大，高并发
* 2 大量的HTTP持久连接（通常基于多线程的请求方式不是持久性连接，每一个的请求需要打开新的连接方式，torando使用同一个TCP连接来发送和接收多个HTTP请求/应答 ）

####C10K问题：



#### tornado使用平台说明：

tornado应该运行在类Unix平台上，因为充分利用linux的epoll工具和BSD的kqueue工具，是tornado不依靠多线程/多进程而达到高性能的原因（BSD是Unix的一个发行版本）

