1、名词解释



    发信者     ------------>    Producer
    收信者     ------------->   Consumer 
    负责暂存  -------------->  Broker
    传输的邮局 -------------> NameServer


启动 RocketMQ 的顺序是先启动 NameServer，再启动 Broker，这时候消 息队列已 经可以提供服务了，想发送消息就使用 Producer来发送，想接收消息 就使用 Consumer来接收 。 很多应用程序既要发送，又要接收，可以启动多个Producer 和 Consumer 来发送多种消息，同时接收多种消息 。




流程图

![img](https://img-blog.csdnimg.cn/20190116140217789.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zODAwMzM4OQ==,size_16,color_FFFFFF,t_70)