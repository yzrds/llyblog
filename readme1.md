### redis
1. 特点
* Redis支持数据的持久化，可以将内存中的数据保存在磁盘中，重启的时候可以再次加载进行使用。
* Redis不仅仅支持简单的key-value类型的数据，同时还提供list，set，zset，hash等数据结构的存储。
* Redis支持数据的备份，即master-slave模式的数据备份。

2. Redis优势
* 原子 – Redis的所有操作都是原子性的，意思就是要么成功执行要么失败完全不执行。单个操作是原子性的。多个操作也支持事务，即原子性，通过MULTI和EXEC指令包起来。


Redis支持五种数据类型：string（字符串），hash（哈希），list（列表），set（集合）及zset(sorted set：有序集合)

redis的一个键最大能存储512MB

每个 hash 可以存储 232 -1 键值对（40多亿）。











































报错
1。redis启动出错Creating Server TCP listening socket 127.0.0.1:6379: bind: No error
解决方法：在命令行中运行

redis-cli.exe

127.0.0.1:6379>shutdown

not connected>exit

然后重新运行redis-server.exe redis.windows.conf，启动成功！