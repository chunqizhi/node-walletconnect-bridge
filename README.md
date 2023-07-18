# WalletConnect Bridge Server

**[DEPRECATED]** Please refer to [walletconnect-monorepo](https://github.com/walletconnect/walletconnect-monorepo) under servers/relay

You can read the old documentation [here](./OLD-README.md)


##

make dev

问题1  
#6 53.02   error: can't find Rust compiler

使用 FROM nginx:1.25.1-alpine

make dev

问题2  
只有 redis 容器启动

使用  
npm install --no-optional  
npm run build  

make dev

问题3  
2023/07/18 06:27:37 [emerg] 1#1: host not found in upstream "node0:5001" in /etc/nginx/servers/localhost.conf:44
nginx: [emerg] host not found in upstream "node0:5001" in /etc/nginx/servers/localhost.conf:44

修改 bridge 为 node

make dev

目前全部正常，访问 

https://localhost/hello

返回  
Hello World, this is WalletConnect v1.0.0-beta