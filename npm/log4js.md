# log4js

#### 使用

```
var log4js = require('log4js');
var logger = log4js.getLogger();
logger.debug("Some debug messages");

```

```
[2010-01-17 11:43:37.987] [DEBUG] [default] - Some debug messages

```


详情

```
var log4js = require('log4js');
//console log is loaded by default, so you won't normally need to do this 
//log4js.loadAppender('console'); 
log4js.loadAppender('file');
//log4js.addAppender(log4js.appenders.console()); 
log4js.addAppender(log4js.appenders.file('logs/cheese.log'), 'cheese');
 
var logger = log4js.getLogger('cheese');
logger.setLevel('ERROR');
 
logger.trace('Entering cheese testing');
logger.debug('Got cheese.');
logger.info('Cheese is Gouda.');
logger.warn('Cheese is quite smelly.');
logger.error('Cheese is too ripe!');
logger.fatal('Cheese was breeding ground for listeria.');

```


#### 参考文献

1. [log4js](https://www.npmjs.com/package/log4js)