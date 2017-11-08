## OpenMPI

本应用提供OpenMPI和C编译环境，打开容器的命令行界面即可执行mpicc、mpirun等命令。工作路径为/work，该目录已经通过samba服务的方式共享给用户，用户可以通过共享文件夹(windows系统)/samba协议(linux系统)的方式进行访问。另外，在/data目录下有一个ping/pong示例程序。

### 访问方式
 1. <a href="javascript:;" onclick="$paraos.openWin('http://172.16.2.189:8080/env/{$T.services[0].accountId}/infra/console?instanceId=1i32214&isPopup=true', 'console', 1000, 700)">打开命令行</a>

 2. 共享文件夹(复制链接，在资源管理器的地址栏中粘贴打开)：
  * 地址：file://172.16.2.183/work，
  * 用户名密码：user/user

### 示例程序
在/data目录下有一个MPI的ping/pong示例程序：mpi-ping.c，可以按如下方式编译成可执行文件

```bash
cd /data
mpicc mpi-ping.c -o ping
./ping -h
```