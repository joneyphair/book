# linux下为用户赋予root权限


#### 添加用户(以gitbook用户举例)

```
useradd gitbook
```

#### 为gitbook用户添加密码
```
passwd gitbook

```

#### 添加gitbook用户到root用户组

```
usermod -g root gitbook

```

#### 修改 /etc/sudoers 文件

找到下面这一行

```
## Allow root to run any commands anywhere
root    ALL=(ALL)     ALL
```

修改为

``` 
## Allow root to run any commands anywhere
root    ALL=(ALL)     ALL
gitbook   ALL=(ALL)     ALL
```


#### 完成
