# 创建Electron 桌面应用


#### 初始化一个项目

```
npm init
```

#### 安装 electron-prebuilt

```
npm install --save-dev electron-prebuilt
```

#### 修改package.json

```
{
  "name": "book",
  "version": "1.0.0",
  "description": "",
  "main": "main.js",
  "scripts": {
     "start":"npm run dev",
     "dev": "./node_modules/.bin/electron ."
  },
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "gitbook": "^3.2.2"
  }
}
```

#### 新建main.js 

```
touch main.js
```

添加内容如下
```

'use strict';


var app = require('app');
var BrowserWindow = require('browser-window');
var mainWindow = null;

app.on('ready', function() {
    mainWindow = new BrowserWindow({
        height: 600,
        width: 800
    });

    mainWindow.loadUrl('http://baidu.com');
    //mainWindow.loadUrl('file://' + __dirname + '/app/index.html');
});

```



#### 相关文章

[用Electron开发桌面应用](http://get.ftqq.com/7870.get)