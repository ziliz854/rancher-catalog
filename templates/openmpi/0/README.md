### 说明

安装OpenMPI和C语言的编译环境。

本应用包含一个MPI的ping/pong测试程序。

```bash
cd /data
mpicc mpi-ping.c -o ping
./ping -h
```