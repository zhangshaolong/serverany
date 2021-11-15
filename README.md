# serverany

任意文件夹的静态服务能力，可以在任意文件夹下启动服务，基于 mock-proxy-middleware 工具，支持 mock 和 proxy 能力的本地静态服务器

```javascript
  // 安装
  npm install serverany -g
  // 启动服务
  serverany --index index.html --base ${pwd} --config config.json --port 8800
```
