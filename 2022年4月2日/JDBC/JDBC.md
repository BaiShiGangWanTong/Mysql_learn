# JDBC是什么？
    Java Databases Connectivity（Java语言链接数据库）

# JDBC的本质？
    JDBC是SUN公司制定的一套接口（interface）
    接口都有调用者和实现者。
    面向接口调用、面向接口写现实类，这都属于面向接口编程。

    为什么要面向接口编程？
        解耦合，降低程序的耦合度，提高程序的扩展力。
        多态机制就是非常典型的：面向抽象编程。（不要面向具体编程）

# 为什么SUN制定一套JDBC接口？
    因为每一个数据库的底层实现都是不同的

# JDBC编程六步
    - 注册驱动（作用：告诉java程序，即将链接的是哪个品牌的数据库）
    - 获取链接（表示JVM的进程和数据库进程之间的通道打开了，这属于进程之间的通信，使用之后一定要关闭）
    - 获取数据库操作对象（专门执行sql语句的对象）
    - 执行SQL语句（DQL,DML）
    - 处理查询结果（只有当第四步执行的是select语句的时候，才有这五步处理查询结果集）
    - 释放资源（使用完资源之后一定要关闭资源，java与数据库属于进程间的通信）