# validate 


#### 安装

```
npm install validate --save-dev
```

#### 使用案例

```

var schema = require('validate');
var user = schema({
  name: {
    type: 'string',
    required: true,
    message: 'Name is required.'
  },
  email: {
    type: 'string',
    required: true,
    match: /+\@.+\..+/,
    message: 'Email must be valid.'
  },
  address: {
    street: {
      type: 'string',
      required: true,
      message: 'Street is required.'
    },
    city: {
      type: 'string',
      required: true,
      message: 'City is required.'
    }
  },
});
 
var errors = user.validate(obj);

```

#### 参考文献



1. [validate](https://www.npmjs.com/package/validate)