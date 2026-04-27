# Frp Service Usage

### 1. Location

The frp service is located under the `/opt/frp/` directory. The directory contains both the server bin and the client bin. The server bin is marked with `s` and the client bin is marked with `c`. In the case, the pi is set as a client so only `frps` files are used. 

``````
 frp/
├── frpc # client bin
├── frpc.toml # client config file
├── frps # server bin
├── frps.toml # server config file
├── LICENSE
└── README.md
``````

### 2. Usage

For adding additional proxies, please visit the [frp official documentation.](https://gofrp.org/zh-cn/docs/)

To use frp as a system service, use the following

``````bash
# 启动frp
sudo systemctl start frpc
# 停止frp
sudo systemctl stop frpc
# 重启frp
sudo systemctl restart frpc
# 查看frp状态
sudo systemctl status frpc
# 设置 frps 开机自启动
sudo systemctl enable frpc
``````

