# 示例展示 
1. 消息发送至消费的过程
2. 消息异常,消息尽最大努力消费(死亡消息除外)
3. 消息处理过程多次消费示例

# 思路
1. 事务业务是否成功以随机数生成(1成功|0失败)
2. 简单的事务处理,消息不清除(Map异常未处理) 
3. 死亡的消息未处理,例子中不做人工处理机制(建议根据业务做一定的处理)

# 中间件
以HashMap代替,完成项目的配置

# 消费者 
处理本地事务为例(线程)

# 生产者
处理本地事务为例(正常事务)

# 监控
直接输出消息情况

# 异常处理(线程)
1. 消息恢复监控,并处理
2. 消息确认监控,并处理
