# AvatarMQ
## AvatarMQ中文简介：

**AvatarMQ是基于Netty构建的分布式消息队列系统，支持多个生产者和多个消费者之间的消息路由、传递。**

* 若干个消费者可以组成一个消费者集群，生产者可以向这个消费者集群投递消息。并且每个消费者只消费自己关注的生产者发送的消息。

* 支持动态新增、删除生产者、消费者。

* 消息投递支持负载均衡策略。

* 消息处理转发服务器（AvatarMQServerStartup）基于异步多线程消息队列进行组织架构，并且和Spring无缝集成。

* 生产者、消费者测试用例参考：com.newlandframework.avatarmq.test包。

* 启动AvatarMQ的消息处理转发服务器（AvatarMQServerStartup）之后，才能进行分布式消息队列系统的消息路由、传递。

* 基于Netty的主从事件线程池模型，网络传输中的消息序列化采用Kryo序列化框架，进一步提升消息序列化性能。
----------
## AvatarMQ English Introduction:

**AvatarMQ is a distributed message queue system based on Netty(java nio framework), which supports message routing and delivery between multiple producers and multiple consumers.**

* A number of consumers can form a consumer cluster, the producer can send messages to this consumer cluster. And each consumer only consumes the message that is sent by the producer.

* To support the dynamic add, delete the producers, consumers.

* Message delivery support load balancing strategy.

* Message processing and forwarding server (AvatarMQServerStartup) based on asynchronous multi thread message queue organization architecture, and seamless integration with Spring.

* Producer, consumer test case reference: com.newlandframework.avatarmq.test package.

* Start AvatarMQ message processing and forwarding server (AvatarMQServerStartup), in order to carry out the distributed message queue system message routing, delivery.

* Based on the Netty master slave event thread pool model, network transmission in the message serialization using Kryo serialization framework, to further enhance the performance of message serialization.
----------
## Author
**唐洁（tangjie）, http://www.cnblogs.com/jietang/**
----------
## License
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html) Copyright (C) 2016 Newland Group Holding Limited
