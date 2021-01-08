# linux常用命令

### 快速过滤配置文件
  grep "^[a-Z|0-9]" wget-log
  
  
### 清除内存
echo 3> /proc/sys/vm/drop_caches

### 查看端口是否启动和相关进程
`
lsof -i:7890
COMMAND   PID USER   FD   TYPE   DEVICE SIZE/OFF NODE NAME

wenjuan 30501  ctd    3u  IPv6 90359550      0t0  TCP *:7890 (LISTEN)

wenjuan 30501  ctd    5u  IPv6 93639798      0t0  TCP pmckutakzv33yayt.novalocal:7890->42.92.190.102:44110 (ESTABLISHED)

`
