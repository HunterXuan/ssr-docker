# docker-ssr

## 使用方法

0x1: 直接使用
```
docker pull hunterxuan/ssr-docker
docker run hunterxuan/ssr-docker:latest -name shadowsocksr -p 443:443
```

0x2: 从当前项目构建(docker-native)
```
git clone https://github.com/HunterXuan/ssr-docker.git
cd ssr-docker
修改 Dockerfile 参数
docker build -t shadowsocksr:latest .
sudo docker run -d --name shadowsocksr -p 本地端口:容器端口

```

0x3: 使用 docker-compose
```
git clone https://github.com/HunterXuan/ssr-docker.git
cd ssr-docker
修改 .env 参数
docker-compose up -d --build

```
