# 🤩 运行 DriveArena 演示！

TrafficManager、WorldDreamer 和 DrivingAgent 之间的通信基于 **FastAPI。WorldDreamer** 和 **DrivingAgent** 可以在**远程服务器**上运行，而 **TrafficManager** 需要在**带有显示器的本地机器**上运行。

## 启动 WorldDreamer 服务

请按照 [README.md](../WorldDreamer/README.md) 准备环境并下载权重。

然后你可以运行以下代码：
```shell
cd WorldDreamer && python tools/dreamer_fast_api.py
```

## 启动 DrivingAgent 服务

请按照 [README.md](../DrivingAgents/UniAD/README.md) 准备环境并下载权重。

```shell
cd DrivingAgents/UniAD && python demo/fast_api_uniad.py --resume=path/to/your/weight
```

## 启动 TrafficManager 并开始模拟
请按照 [README.md](../TrafficManager/README.md) 启动模拟。

如果一切顺利，你将看到一个类似这样的窗口!
![alt text](../assets/simulation.png)