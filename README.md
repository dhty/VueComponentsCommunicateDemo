# vuejs-demo
实现了vuejs组件之间的通讯问题

在Vue的官方文档中，只有父子之间通信的例子，并无两个独立组件之间通信的例子。

在某种场合下，如改变组件A的状态，会触发组件B某状态的切换，这种时候就需要用到组件间通信的方法。

官方推荐vuex，但是其学习成本较高，在非大型应用中使用vuex并非上策，于是在现有资源下研究出了此方法。

此方法的核心思想就是子组件之间不直接通信，而是通过其共同的父组件作为中转站，把数据统一发送到父组件，再由父组件定向把内容分发给相应的子组件，实现了相互独立的子组件之间通信的需求。
