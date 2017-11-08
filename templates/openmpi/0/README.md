### 说明

安装OpenMPI和C语言的编译环境。

本应用提供OpenMPI和C编译环境，打开容器的命令行界面即可执行mpicc、mpirun等命令。工作路径为/work，该目录已经通过samba服务的方式共享给用户，用户可以通过共享文件夹(windows系统)/samba协议(linux系统)的方式进行访问。另外，在/data目录下有一个ping/pong示例程序。

示例程序：
```bash
cd /data
mpicc mpi-ping.c -o ping
./ping -h
```