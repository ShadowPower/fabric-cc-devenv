# Hyperledger Fabric Chaincode 开发环境

这是一个易于使用的，使用 CouchDB 作为状态数据库的，支持多模块的 Hyperledger Fabric Chaincode 开发测试环境。

使用前请先获取所有 Hyperledger Fabric 的 Docker 镜像。



## 使用说明：

1. 将您的 chaincode 工程文件夹放置到 chaincode 目录里；

2. 把最外层目录当做 GOPATH 根目录看待，修改您的 import 语句，您的项目根目录应为 "chaincode/项目名"；

3. 打开终端模拟器，执行 ./start.sh 启动环境；

4. 新建一个标签，执行 ./chaincode.sh 进入 chaincode 安装/运行环境，您可以下载第三方模块，编译并运行您的 chaincode。详情请参阅官方文档；

5. 新建一个标签，执行 ./cli.sh 进入 chaincode 测试环境，您可以安装，初始化并测试您的 chaincode。详情请参阅官方文档；

6. 使用结束后，返回第一个标签，执行 ./start.sh 停止所有 docker 实例，删除所有容器和网络。

   ​