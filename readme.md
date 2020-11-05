
实现一个分布式缓存

一：LRU 缓存淘汰策略 
二：单机并发缓存 
三：HTTP 服务端 
四：一致性哈希(Hash) 
五：分布式节点 
六：防止缓存击穿 
七：使用 Protobuf 通信 


结构
```
 cache/
    |--lru/
        |--lru.go  // lru 缓存淘汰策略
    |--byteview.go // 缓存值的抽象与封装
    |--cache.go    // 并发控制
    |--dtbCache.go // 负责与外部交互，控制缓存存储和获取的主流程
```