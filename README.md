# serverany

任意文件夹的静态服务能力，可以在任意文件夹下启动服务，基于 mock-proxy-middleware 工具，支持 mock 和 proxy 能力的本地静态服务器

```javascript
  // 安装
  npm install serverany -g
  // 启动服务
  serverany --index index.html --base ${cwd} --config config.js --port 8800

--index 配置访问的页面地址，默认值index.html，即在--base文件夹下的index.html
--base 获取相对地址的基准路径，默认为执行serverany的目录
--config mock proxy配置文件地址，默认为config.js，即在--base文件夹下的config.js，具体配置请参考mock-proxy-middleware
--port 默认的服务端口，默认http端口为8800，https端口基于http端口+1

注意：如果配置的路径以“/”开头，那么认为是绝对地址，不再基于--base进行查找。
```