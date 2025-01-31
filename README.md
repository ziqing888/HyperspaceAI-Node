# HYPERSPACE 节点加入指南




## • 筹集资金： 5500 万美元
简介：

@HyperspaceAI正在构建一个基于浏览器的区块链超级计算机，旨在为用户提供安全、可控的人工智能应用程序。

## 加入步骤
访问官方网站
首先，打开您的浏览器并访问以下网址：

http://node.hyper.space

GitHub： http://github.com/hyperspaceai

## 2. 激活节点
1：在箭头 1 处选择模型 在箭头2找到并打开红色开关。此操作后，会弹出一条消息：“已分配并准备好接受挑战”。系统将自动进行配置设置。请耐心等待几分钟，直到配置完成。
![image](https://github.com/user-attachments/assets/8b09a421-a6fb-4a78-9547-6fd5fa3a8508)


2：可以选择以下两种方式之一来运行您的节点：
使用浏览器： 直接在浏览器中运行节点，无需下载任何额外的软件。
下载 Hyperspace 应用程序： 若您更喜欢使用专用应用程序，可以下载并安装 Hyperspace 应用程序。

3. 提高活跃度

为了确保您的节点保持活跃并获得更高的评分，请确保以下几点：
保持在线： 节点需要持续在线，以便处理网络请求和挑战。这将直接影响您的活跃度分数。
完成所有活动： 定期检查并完成平台要求的各项活动，以维持和提升您的节点评分。

注意：该项目对 RAM 和计算资源的需求较高，依赖用户共享 RAM 进行数据计算。如果您的设备性能较低，请谨慎参与，以免影响设备运行。

# .Linux CLI 节点 （VPS）
系统要求
最低配置：

4GB 内存，2 个虚拟 CPU
推荐配置：

8GB 内存，4 个虚拟 CPU

使用 Docker 运行：
一键运行脚本
```
curl -O https://raw.githubusercontent.com/ziqing888/HyperspaceAI-Node/refs/heads/main/start_aios.sh && chmod +x start_aios.sh && ./start_aios.sh
```
按照提示输入私钥即可

## 有用的命令
查看日志：
```
docker logs -f aios-container
```
查看积分：
```
docker exec -it aios-container /app/aios-cli hive points
```
查看私钥：
```
docker exec -it aios-container /app/aios-cli hive whoami
```
## 项目结束后
停止 Docker 容器：
```
docker stop aios-container
```
删除 Docker 容器：
```
docker rm aios-container
```
删除 Docker 镜像：
```
docker rmi kartikhyper/aios
```

