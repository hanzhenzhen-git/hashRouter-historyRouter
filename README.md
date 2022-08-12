# hashRouter-historyRouter
hash路由和history路由的原理

## 介绍
   * 单页面富应用(SPA)提高了web应用的交互体验。在与用户交互过程中，url改变也不需要向服务器请求新的静态资源，页面显示变得更加流畅。SPA需要通过前端路由改变页面显示内容。
   * 前端路由的核心：
      * 改变url，但是页面不进行刷新
      * 自己监听url的改变，根据url的改变自己改变页面的内容
   * url改变，同时不引起页面刷新有两个办法
      * 通过hash改变url
      * 通过h5中的history模式改变url
   * url的hash，本质上监听location对象的hash值变化事件来实现
   * history是利用浏览历史记录栈的API实现
      

## hash路由和history路由的优缺点
   * hash的优势时兼容性好，低版本IE都能运行；缺点是url中会有一个'#'号，显得不像真实路径
   * history优势是url更优雅，缺点是不兼容低版本浏览器

