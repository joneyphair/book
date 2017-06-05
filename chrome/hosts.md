# hosts 修改不生效


#### 

```
chrome://net-internals/#DNS
```


####  修改Hosts不生效的根本原因

服务器在响应头设置了 Connection: keep-alive （一般的网页都会设置 keep-alive，保持长连接，避免多次连接产生网络消耗）之后，客户端会跟服务器保持长连接，只要长连接不断开，页面在请求的时候就不会重新解析域名！


```
chrome://net-internals/#sockets
```

点击 close idle sockets 按钮,尝试清除