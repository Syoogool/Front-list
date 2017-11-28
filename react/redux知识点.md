## 基础
1. redux的三个原则
2. action
3. reducer
4. store



## 进阶
### middleware(中间件）
  **提供在action发起之后，到达reducer之前的的扩展点添加功能，比如日志，错误报告，调用异步接口，路由**

- [demo](https://codesandbox.io/s/ko5vkj18oo)
- [redux中文文档-中间件](http://cn.redux.js.org//docs/advanced/Middleware.html)


常用中间件
- redux-logger 


- redux-thunk
    
    提供 action creators 返回函数（之前的action只能是对象，从而提供异步action

- redux-promise

   提供action createors 返回promise对象
 
 
## redux-dom
1. Provider
2. Connect



## redux-router-dom

