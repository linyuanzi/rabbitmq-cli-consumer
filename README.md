# RabbitMQ cli consumer 定制化
项目介绍： https://github.com/linyuanzi/rabbitmq-cli-consumer

## 已完成
- The executable: 可指定执行目录
```
# 如指定到/tmp目录执行php think命令
./rabbitmq-cli-consumer -e "/tmp php think"
```

- 实现队列连接参数通过环境变量获取
```
# 命令行执行参数
$ ./rabbitmq_cli_cunsumer --env-code CONFIG

# 环境变量(CONFIG前缀对应--env-code参数)
export CONFIG_MQ_DELAY_EXCHANGE_NAME=""
export CONFIG_MQ_PASSWORD=""
export CONFIG_MQ_PORT=""
export CONFIG_MQ_QUEUE_NAME=""
export CONFIG_MQ_HOST=""
export CONFIG_MQ_VHOST=""
export CONFIG_MQ_ROUTE_KEY=""
# export CONFIG_MQ_DELAY_ROUTE_KEY=""
# export CONFIG_MQ_DELAY_QUEUE_NAME=""
export CONFIG_MQ_EXCHANGE_NAME=""
export CONFIG_MQ_USER=""
```

## 执行命令参考
```
./rabbitmq_cli_cunsumer --env-code CONFIG -e "/disk/projects/A312/api php think  GolangConsumer --body"  -V  --strict-exit-code -m -o
```

## 进一步扩展方向(局限)
- 实现同时监听多个vhost