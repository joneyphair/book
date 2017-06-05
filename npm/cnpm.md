# cnpm 安装



#### 使用cnpm

```
npm install -g cnpm --registry=https://registry.npm.taobao.org

```

#### 或者你直接通过添加 npm 参数 alias 一个新命令

```
echo '\n#alias for cnpm\nalias cnpm="npm --registry=https://registry.npm.taobao.org \
  --cache=$HOME/.npm/.cache/cnpm \
  --disturl=https://npm.taobao.org/dist \
  --userconfig=$HOME/.cnpmrc"' >> ~/.zshrc && source ~/.zshrc
```