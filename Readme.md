#模拟数据

1. `mockData`模拟数据文件夹，可在该文件夹下创建多个json数据

2. `src/server.js`服务启动文件,可修改服务端口
  
   监听端口 `prot`可随意修改
   >```javascript
   >const port = 20000
   >app.listen(port, () => 
   >    console.log(`本机服务已启动>>> http://${getIP()}:${port}`)
   >);
   >```
   
3. 启动项目

   ```shell
   # 同步依赖
   npm install
   # 启动项目
   npm serve
   ```