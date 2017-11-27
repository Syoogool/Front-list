## 基础
1. <Router>
2. <Link>
3. <Route>
  这是React-Router4中最重要的组件，最基本的职责就是当当前访问的地址（location）和 Route中path 匹配时，
  就渲染对应的UI界面。
  <Route>自带三种渲染方法和三个对应的propso:
  - <Route component> match
  - <Route render> location
  - <Route children> history
  
  每种渲染方式都应用于特定场景，大部分情况下使用component
  
4. <NavLink>
5. <Redirect>
6. <Switch>


## 进阶
- [react-router的实现原理](https://segmentfault.com/a/1190000004527878)
