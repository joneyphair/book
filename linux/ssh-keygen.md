# ssh-keygen 生成密钥


#### 生存密钥：

```
ssh-keygen -t rsa -C "gitbook@github.com"
```

按3个回车，密码为空。

```
Your identification has been saved in /home/tekkub/.ssh/id_rsa.
Your public key has been saved in /home/tekkub/.ssh/id_rsa.pub.
The key fingerprint is:
………………
```

得到了两个文件：id_rsa(私钥）、id_rsa.pub（公钥)
