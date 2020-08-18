#模拟数据

1. `mockData`模拟数据文件夹，可在该文件夹下创建多个json数据

2. `src/router/api.js` 创建模拟api文件
      
    此处用于读取`mockData`下的json文件
    >```javascript
    >const data = require('./mockData/data.json')
    >```
   
    设置请求接口 `all`任何请求类型都可 `data`为上方引入文件常量
    >```javascript
    >app.all('/api/data', (req, res) => res.send(data));
    >```
      
    以上可引入多文件，创建多个接口请求，目前请求类型只测试 `get` `post` 可行
    
3. `src/server.js`服务启动文件,可修改服务端口
  
   监听端口 `prot`可随意修改
   >```javascript
   >const port = 20000
   >app.listen(port, () => 
   >    console.log(`本机服务已启动>>> http://${getIP()}:${port}`)
   >);
   >```
   
4. 启动项目

   ```shell
   # 同步依赖
   npm install
   # 启动项目
   npm serve
   ```