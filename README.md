# RabbitMQ cli consumer 定制化
项目介绍： https://github.com/linyuanzi/rabbitmq-cli-consumer

## 已完成
- The executable: 可指定执行目录
```
# 如指定到/tmp目录执行php think命令
./rabbitmq-cli-consumer -e "/tmp php think"
```

## 进一步扩展方向(局限)
- 实现队列连接参数通过环境变量获取
- 实现同时监听多个vhost