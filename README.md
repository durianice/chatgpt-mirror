# 蟑螂代理

## 主程序
[https://github.com/cockroachai/cockroachai](https://github.com/cockroachai/cockroachai)

## 代理程序
[https://github.com/cockroachai/ja3-proxy](https://github.com/cockroachai/ja3-proxy)

## 运行步骤
### 1. 安装 docker 和 docker-compose (略)
### 2. 下载配置文件
```bash
git clone https://github.com/durianice/chatgpt-mirror.git
```
### 3. 编辑配置文件
```bash
cd chatgpt-mirror/proxy && cp .env.example .env && vi .env
```
> `REAL_IP` 和 `CLIENTKEY` 必填，其他可以默认
### 4. 测试代理连通性
`curl --insecure --proxy http://cat:cute@x.x.x.x:9988 'https://chat.openai.com/'`
### 5. 配置蟑螂 PROXY 字段
PROXY=http://cat:cute@x.x.x.x:9988
### 6. 启动蟑螂
### 7. 其他配置请查看原文档

## 感谢
维护不易，请支持原开发者 [https://github.com/cockroachai](https://github.com/cockroachai)
