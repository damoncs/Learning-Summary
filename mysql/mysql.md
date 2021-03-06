###MySQL
####mysql存储引擎及面向的数据库应用
在MySQL中，存储引擎的概念相比其他数据库尤为重要，对于每个存储引擎可能面向一种特定或者最优的数据库应用环境。

MySQL由以下几部分组成：

- 连接池组件
- 管理服务和工具组件
- SQL接口组件
- 查询分析器组件
- 优化器组件
- 缓冲组件
- 插件式存储引擎
- 物理文件

下面总结列出了常见的存储引擎及他们面向的数据库应用：

- InnoDB存储引擎：支持事务，主要面向联机事务处理（OLAP）的应用。

特点是：行锁设计，支持外键

- MyISAM存储引擎：不支持事务、表锁设计、支持全文索引，主要面向OLAP应用

另一点不同：它的缓冲池只缓存索引文件，而不缓存数据文件，这与大多数的数据库不同。

- NDB存储引擎：是一个集群存储引擎。