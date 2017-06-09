# node 使用babel


#### 初始化项目

```
npm init node-babel

```

#### 安装相关插件


```
npm install --save-dev babel babel-core babel-preset-es2015 babel-preset-stage-2

```

#### packge.json 内容

```
{
  "name": "node-babel",
  "version": "1.0.0",
  "description": "",
  "scripts": {
    "start": "./node_modules/.bin/nodemon ./index.js",
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "babel": "^6.23.0",
    "babel-cli": "^6.24.1",
    "babel-core": "^6.25.0",
    "babel-preset-es2015": "^6.24.1",
    "babel-preset-stage-2": "^6.24.1",
    "nodemon": "^1.11.0",
  },
  "main": "index.js"
}

```

#### 配置.babelrc文件

```
 {
    "presets": [
      "es2015",
      "stage-2"
    ],
    "plugins": []
}

```



#### 项目入口文件内容

index.js

```
require('babel-core/register');	
require('./src/index.js');

```


#### 业务代码 在src/index.js 

```
import express from 'express'

```

