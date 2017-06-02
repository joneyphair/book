# npm 安装插件常规错误解决方案


#### 1. 安装包爆错

```
[sqlite3] Success: "/usr/local/lib/node_modules/jsbin/node_modules/sqlite3/lib/binding/node-v11-darwin-x64/node_sqlite3.node" is installed via remote
npm ERR! Darwin 14.1.0
npm ERR! argv "node" "/usr/local/bin/npm" "i" "-g" "jsbin"
npm ERR! node v0.10.40
npm ERR! npm  v2.12.1
npm ERR! path /Users/cdelvasto/.npm/connect/2.7.2
npm ERR! code EACCES
npm ERR! errno 3

```
解决方式：
在终端执行如下命令:

```
sudo chown -R $(whoami) "$HOME/.npm"
npm -g install npm

```