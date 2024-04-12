# seckill-project

秒杀请求首先到达负载均衡，负载均衡转发到适合的网关，网关服务鉴权通过后路由到秒杀服务，秒杀服务校验参数通过后查询商品信息，商品信息没有问题则进行库存预扣减，扣减成功生成订单信息。

![seckill_framework](assets/seckill_framework.png)