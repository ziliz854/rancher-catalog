# Hadoop + Yarn (试验性)


### Info:
 该模板将安装Apache Hadoop 2.7.1 和 Yarn，建议运行在至少8GB内存的主机上。由于使用了命名卷，要求Docker版本最低为1.9.x（如1.9.1），一个环境可以部署一个Hadoop集群实例，支持给集群增加额外节点，暂不支持移除节点。
 
### Using

从应用商店选择Hadoop，支持设置常用的HDFS选项和Yarn/MapReduce 内存选项。

设置完选项后即可部署集群。

你可以通过以下服务来访问：

* HDFS 管理: `namenode-primary:50070`.
* Yarn Resource manager: `yarn-resourcemanager:8088` 

HDFS文件系统URL: `hdfs://<namenode>:8020`
