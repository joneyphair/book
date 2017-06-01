## 新建gitbook项目

#### 1. 安装gitbook-cli
```
npm install -g gitbook-cli
```

#### 2. 初始化项目

```
gitbook init demo-book
```


#### 3. 启动浏览

```
gitbook serve
```

#### 4. 构建_book目录（存放各种html文件)

```
gitbook build
```

### 3. 使用局部gitbook命令

```
npm init
npm install --save-dev gitbook
```
修改package.json文件

```
{
  "name": "book",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "./node_modules/.bin/gitbook serve",
    "build": "./node_modules/.bin/gitbook build"
  },
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "gitbook": "^3.2.2"
  }
}
```

#### 完成

