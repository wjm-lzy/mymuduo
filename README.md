手写muduo网络库
使用epoll多路IO复用
1）调用epoll_create()建立一个epoll对象（在epoll文件系统中为这个句柄对象分配资源）
2）调用epoll_ctl向epoll对象中添加这100万个连接的套接字
3）调用epoll_wait收集发生的事件的fd资源

使用LT方式触发：即如果不进行处理，就会一直通知
