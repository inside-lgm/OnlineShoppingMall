
## 一、项目介绍
项目实现商品的从后台填写商品信息、商品上架（立即上架 或 定时上架），到前台用户可见可商品后进行购买（购物车 或 立即购买）后的待结算、待支付状态，再到用户支付（模拟支付，暂时没有实现）后商品的状态为待发货，后台管理人员进行发货操作后填写运单号码并确认发货，再到用户收到商品后点击确认收货、评价订单，最后订单状态已完成的整个在线购物的商品交易流程。

* 商品上架-> 待结算 ->待支付 ->待发货 ->待收货 ->待评价 ->已完成


##二、技术栈
* Spring + SpringMVC + MyBatis + Redis + RabbitMQ + Quartz + Bootstrap

* 后端使用 SSM 作为主框架进行开发，集成 Redis 内存缓存、RabbitMQ 消息队列和 Quartz 作业调度框架。

* 前端使用 JSP 和 Bootstrap 来进行项目开发。



## 三、项目亮点
* 1）使用 Spring + SpringMVC + MyBatis + Redis + RabbitMQ + Quartz + Bootstrap 进行项目整合开发

* 2）使用 Redis 实现购物车功能和商品信息的数据缓存功能，提高系统的响应速度并降低数据库的访问压力

* 3）使用 RabbitMQ 实现订单的异步化处理和系统的日志处理，提升系统对用户操作的响应速度并降低模块之间的耦合程度

* 4）使用 Spring AOP 在不侵入系统代码的基础上实现系统的日志收集、权限校验和数据埋点等功能

* 5）使用 Quartz 实现商品的自定义定时上架功能，为用户提供更高的操作灵活性

