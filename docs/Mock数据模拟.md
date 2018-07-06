# Mock数据模拟

在iview-admin2.0中使用[Mock.js](http://mockjs.com/)来实现AJAX请求拦截并返回模拟数据，方便前端开发人员的快速开发，无需等待后端接口实现。

已用户信息相关接口为例来做介绍，我们的Mock配置都在`./src/mock`文件夹下，首先在`index.js`文件中注册url匹配规则，并且设置匹配后的处理回调。
```javascript
// 将login相关的处理回调引入
import { login } from './login'
// 配置拦截匹配规则和处理回调
Mock.mock(/\/login/, login)
```

然后在login.js文件中定义处理回调，如下
```javascript
export const login = req => {
  req = JSON.parse(req.body)
  return {
    code: 200,
    data: {token: USER_MAP[req.userName].token},
    msg: ''
  }
}
```
