## 创建项目easy_npm

### 初始化npm

    {code}npm init{code}

    按照提示输入相关信息

### index.js 实现逻辑， 这里测试一个简单类

```javascript
'use strict'

class NpmTest{

    constructor(){

    }

    greet() {
        return 'hello npm2'
    }

}

module.exports = NpmTest;
```

## 发布包

### 注册www.npmjs.com账号

### console添加npm 账号
```
npm adduser
```

### 查看当前登录的账号

```
npm whoami
```
### 发布到公共服务器

参考 

[参考文档](https://docs.npmjs.com/cli/publish)

这里npm publish就可以，因为填写了package.json信息

### 可能出现的问题

#### 版本过低

```
npm ERR! Error: forbidden may not mix password_sha and pbkdf2
```

升级npm

```
npm install npm -g
```

#### 发布不上去

确保npm配置的是 registry=https://registry.npmjs.org/， 而不是其他镜像

更改配置 ~/.npmrc 

## 发布升级包

更改package.js 版本号， npm publish
