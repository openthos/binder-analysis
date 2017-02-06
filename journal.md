# 2017年2月5日

https://github.com/hungys/binder-for-linux
试图重现它的操作。

git clone
编译

void value not ignored as it ought to be
ret = misc_deregister(&binder_miscdev);

https://forums.virtualbox.org/viewtopic.php?f=7&t=70150
因为 linux kernel 4.3 之后 misc_deregister return void

修改后编译成功

运行测试
成功

![image](https://github.com/openthos/binder-analysis/blob/master/raw/2017-2-5Image.png)
binder是字符设备

![image](https://github.com/openthos/binder-analysis/blob/master/raw/2017-2-5Image1.png)
在Android上也是字符设备

所以杂项设备属于字符设备


