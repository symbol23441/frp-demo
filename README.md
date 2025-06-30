# frp-demo
本项目是frp的一个使用测试demo

## 1、命令行执行

官网下载frp包: https://github.com/fatedier/frp/releases

frpc.toml、frpc.toml分别是服务器端和内网端的配置示例。 命令行如下运行：

服务器端：`./frps -c frps.toml` 

 	或后台运行：`nohup ./frps -c frps.toml > frps.log 2>&1 &`

内网端:`./frpc -c frpc.toml`

​	或后台运行：`nohup ./frpc -c frpc.toml > frpc.log 2>&1 &`

## 2、docker运行

docker-frps 外网服务器端的docker compose配置
docker-frpc 内网端的docker compose配置

## 3、简单服务测试

8080SpringbootTest.jar 是一个简单端口服务，用于测试frp测试。
测试地址：http://localhost:8080/

java -DPORT=9000 8080SpringbootTest.jar
可通过-DPORT重新设置窗口
java -DPORT=9000 8080SpringbootTest.jar



附件：

[frp-demo博客]: https://symbol23441.github.io/2025/06/30/%E5%86%85%E7%BD%91%E7%A9%BF%E9%80%8F-by-ssh-or-frp/

