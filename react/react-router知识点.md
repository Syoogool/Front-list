## 基础
###  &lt;Router&gt;


###  &lt;Link&gt;
**提供申明式，无障碍的导航**

- to: string  导航到指定的位置
```javascript
<Link to="/courses/">
```

- to: object 携带参数的导航
```javascript
<Link to={{
  pathname: '/courses',
  search: '?sort=name',
  hash: '#the-hash',
  state: { fromDashboard: true }
}}/>
```

### &lt;NavLink&gt;
  特殊版的&lt;Link&gt;,**匹配到当前地址将向渲染元素添加样式属性（激活状态）**
  
- activeClassName: string  
 导航激活应用的样式名
 ```javascript
 <NavLink to="/faq" acriveClassName="selected">FAQS</NavLink>
 ````
 - activeStyle: object
  直接写styled对象
```javascript
 <NavLink
  to="/faq"
  activeStyle={{
    fontWeight: 'bold',
    color: 'red'
   }}
>FAQs</NavLink
 ````
 
### &lt;Redirect&gt;
 **导航到一个新地址，并且新地址将覆盖历史纪录中的当前地址**

- to: string
- to: object
 和&lt;Routet&gt;中to用法一样
 
 
 
###  &lt;Switch&gt;
 **只渲染第一个与当前访问地址匹配的&lt;Route&gt;或&lt;Redirect&gt;**
  这个看官网实例  使用场景可以是侧边栏 面包屑 动画转场


###  &lt;Route&gt;
   这是React-Router4中最重要的组件，最基本的职责就是**当当前访问的地址（location）和 Route中path 匹配时，
  就渲染对应的UI界面。**
  
  自带三种渲染方法和三个的props对象:
  
  - &lt;Route component&gt;
  - &lt;Route render&gt;
  - &lt;Route children&gt;
  
  每种渲染方式都应用于特定场景，大部分情况下使用component
  
  三个props:
  1. match
  **match对象包含了&lt;Route path&gt;如何与URL匹配的信息**
  2. location
  **表示当前的位置，要导航到的我地址，访问过的地址**
     如下是一个location对象实例
     ```javascript
     {
       key: 'ac3df4', // not with HashHistory!
       pathname: '/somewhere'
       search: '?some=search-string',
       hash: '#howdy',
       state: {
         [userDefined]: true
       }
     }
     ```
  3. history  **实现多种历史对话管理**
  
   - browser history   HTML5 history在DOM上实现
   - hash history  旧版浏览器 hisroty在DOM上实现
   - memory history  history在内存上实现 用于测试或者非DOM环境
   
   history通用属性和方法
  
  每个渲染方式都将传入这三种props
  
###  &lt;Prompt&gt;
  ** 当用户离开当前页面的提示**

## 进阶
- [react-router的实现原理](https://segmentfault.com/a/1190000004527878)
