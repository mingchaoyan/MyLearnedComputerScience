# Operating System

## 进程管理

### 相关命令

* 查看端口对应进程
```
lsof -i :6379
```

## 文件管理

### 外存分配方式
* FAT(File Allocation Table)
    - 单文件最大 4GB
* NTFS(New Technology File System)
    - 受最大分割容量限制
* exFAT(Extended File Allocation Table File System)
    - 单文件最大 16EB(1EB=1024P=1024*1024T)

### 权限

#### 文件
* r 读取文件的实际内容
* w 编辑
* x 执行

#### 目录
* r 读取目录结构列表
* w 异动目录结构列表（新建文件／目录，删除文件目录，更名）
* x 用户能否进入该目录作为工作目录(cd)

## 操作系统接口

### Shell

#### 命令 
##### sudo 只能对可执行文件有效，对 shell 内嵌命令无效
* 解决方案1
```
sudo sh -c "cd /path/to/dir"
```
* 解决方案2
切到root操作
