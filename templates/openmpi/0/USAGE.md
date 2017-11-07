## OpenMPI

本应用提供OpenMPI和C编译环境，打开容器的命令行界面即可执行mpicc、mpirun等命令。工作路径为/work，该目录已经通过samba服务的方式共享给用户，用户可以通过共享文件夹(windows系统)/samba协议(linux系统)的方式进行访问。另外，在/data目录下有一个ping/pong示例程序。

### 访问方式
 * <a href="{$T.publicEndpoints.jupyter_6006.url}" target="_blank">打开命令行</a>
 * <a href="\\172.16.2.183\work" target="_blank">共享文件夹</a>，用户名/密码：user/user

### 示例程序
在/data目录下有一个MPI的ping/pong示例程序：mpi-ping.c，可以按如下方式编译成可执行文件

```bash
cd /work
mpicc mpi-ping.c -o ping
./ping -h
```