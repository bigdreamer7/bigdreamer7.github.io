# 系统调用
[`strace`](https://strace.io)工具可以用于监控和篡改进程与Linux内核之间的交互，包括系统调用、信号传递和进程状态的更改。
```sh
$ strace -p 26380
strace: Process 26380 attached
...
```
常用参数：
* `-f` : 同时追踪子进程或子线程的系统调用
* `-e` : 过滤追踪的系统调用类型
```sh
-e trace=%clock    Trace all system calls that read or modify system clocks.
         %creds    Trace all system calls that read or modify user and group identifiers or capability sets.
         %desc     Trace all file descriptor related system calls.
         %file     Trace all system calls which take a file name as an argument.
         %fstat    Trace fstat and fstatat syscall variants.
         %fstatfs  Trace fstatfs, fstatfs64, fstatvfs, osf_fstatfs, and osf_fstatfs64 system calls.
         %ipc      Trace all IPC related system calls.
         %lstat    Trace lstat syscall variants.
         %memory   Trace all memory mapping related system calls.
         %network  Trace all the network related system calls.
         %process  Trace all system calls which involve process management.
         %pure     Trace syscalls that always succeed and have no arguments.
         %signal   Trace all signal related system calls.
         %stat     Trace stat syscall variants.
         %statfs   Trace statfs, statfs64, statvfs, osf_statfs, and osf_statfs64 system calls.
         %%stat    Trace syscalls used for requesting file status.
         %%statfs  Trace syscalls related to file system statistics.
```
* `-o` : 输出结果到文件
