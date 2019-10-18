# unpv22e
learn unpv22e

```
cd unpv22e
./configure
cd lib
make

```

## Q:
* 遇到下面：修改unpipc.h第115行。unpipc.h中把115 内容注释掉。再次编译
```
    /usr/include/stdint.h:49: 错误：重复的 'unsigned'
    /usr/include/stdint.h:49: 错误：声明指定了两个以上的数据类型
    /usr/include/stdint.h:50: 错误：重复的 'unsigned'
    /usr/include/stdint.h:50: 错误：重复的 'short'
    /usr/include/stdint.h:52: 错误：重复的 'unsigned'
    /usr/include/stdint.h:52: 错误：声明指定了两个以上的数据类型
    make: *** [daemon_inetd.o] 错误 1
```
* 遇到下面：把unpipc.h中第479，480行注释掉。再次编译
```
    In file included from daemon_inetd.c:1:
    unpipc.h:479: 错误：expected '=', ',', ';', 'asm' or '__attribute__' before '*' token
    unpipc.h:480: 错误：expected ')' before '*' token
```
* 遇到下面：修改 unpv22e/Make.defines中的LIB_OBJS的".o"文件，删除"wrapsunrpc.o"
```
    wrapsunrpc.c:3: 错误：expected '=', ',', ';', 'asm' or '__attribute__' before '*' token
    wrapsunrpc.c:16: 错误：expected ')' before '*' token
    make: *** [wrapsunrpc.o] 错误 1
```
