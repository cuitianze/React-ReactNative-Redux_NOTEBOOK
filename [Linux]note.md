[Linux工具快速教程](http://linuxtools-rst.readthedocs.io/zh_CN/latest/index.html)

[查看目录下文件个数]
```
ls -l |grep "^-"|wc -l
```

[查看目录内文件大小并排序]
```
du -sh * | sort -n
```

[以上命令结合grep能得到行号]
```
du -sh * | sort -n | grep 0 -n
```
