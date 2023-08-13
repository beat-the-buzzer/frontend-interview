## 双向绑定的原理

v-model ==> value="xx" @input/@change

ViewModel为model和view之间的桥梁：监听模型数据的改变和控制视图行为、处理用户交互。

## Vue Router 的 hash 和 history 有什么区别，实现原理

hash 模式是一种把前端路由的路径用井号 # 拼接在真实 url 后面的模式。当井号 # 后面的路径发生变化时，浏览器并不会重新发起请求，而是会触发 onhashchange 事件。

pushState() 设置的新 URL 可以是与当前 URL 同源的任意 URL；而 hash 只可修改 # 后面的部分，因此只能设置与当前 URL 同文档的 URL；

history 模式下，前端的 URL 必须和实际向后端发起请求的 URL 一致，需要服务器端做额外的配置，否则会出现刷新404的情况。
