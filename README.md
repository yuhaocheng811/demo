# Server Side Rendering

* ### 前端渲染和后端渲染

[后端渲染步骤](https://ss.csdn.net/p?https://mmbiz.qpic.cn/mmbiz_png/aVp1YC8UV0eQGicogk1hYedJfRuVIXhM9yvUa1mf0zp2Tjv0bIrNP9QuFsb3LpVFtiaHhVeEE0hQibKNW02eEiadvA/640?wx_fmt=png)

1.前端请求一个地址 url

2.后端接收到这个请求，然后根据请求信息，从数据库或者其他地方获取相应的数据

3.使用模板引擎（如 java>jsp、 php>smarty）将这些数据渲染成 html

4.将 html 文本返回给前端
> 后端渲染HTML的情况下，浏览器会直接接收到经过服务器计算之后的呈现给用户的最终的HTML字符串，这里的计算就是服务器经过解析存放在服务器端的模板文件来完成的，在这种情况下，浏览器只进行了HTML的解析，以及通过操作系统提供的操纵显示器显示内容的系统调用在显示器上把HTML所代表的图像显示给用户。

> 好处：前端耗时少（前端只负责将html进行展示），利于SEO

> 坏处：网络传输数据量大，占用（部分、少部分）服务器运算资源，response 出的数据量会（稍）大点，模板改了前端的交互和样式什么的一样得跟着联动修改

[客户端渲染步骤](https://ss.csdn.net/p?https://mmbiz.qpic.cn/mmbiz_png/aVp1YC8UV0eQGicogk1hYedJfRuVIXhM9ic7qOSh4MHR15TfUDmPo7dRmY18kY5adcNqno5xicN9s5SMO7EicJpQYQ/640?wx_fmt=png)

1.前端请求一个地址 url

2.后端接收到这个请求，然后把相应的 html 文件直接返回给前端

3.前端解析 js 后，然后通过 ajax 向后台获取相应的数据

4.由 js 将这些数据渲染成页面

> 前端渲染的方式起源于JavaScript的兴起，ajax的大热更是让前端渲染更加成熟，前端渲染真正意义上的实现了前后端分离，前端只专注于UI的开发，后端只专注于逻辑的开发，前后端交互只通过约定好的API来交互，后端提供json数据，前端循环json生成DOM插入到页面中去。

> 好处：网络传输数据量小（减少了服务器压力）

> 坏处：前端耗时较多，不利于SEO

*****

* ### 服务器端渲染模板

*****

* ### Nuxt.js

  #### 1.nuxt脚手架create-nuxt-app 初始化项目模板 项目结构
  #### 2.基本路由 动态路由 路由参数校验 嵌套路由
  #### 3.布局组件 error布局组件
  #### 4.全局样式引入
  #### 5.异步数据获取 axios
  #### 6.SEO优化

*****

* ### Next.js
