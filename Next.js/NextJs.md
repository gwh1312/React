Next.js介绍 
Next.js是一个轻量级的React服务器端渲染应用框架，有了它我们可以轻松的实现React的服务器端渲染，从而加快首屏打开速度，也可以做SEO（搜索引擎优化）。
解决了我们什么问题
1.完善的React项目架构，搭建轻松
2.解决服务器端渲染
3.丰富的插件
4.灵活的配置

创建项目
一、手动创建步骤
1. 创建文件夹
```
E:
mkdir NextDemo
npm init
```
2. 安装所需依赖包
使用yarn安装
``` 
yarn add react react-dom next
```
也可以使用npm安装
```
npm install --save react react-dom next
```
3. 增加快捷命令
在package.json中配置
```
 "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev" : "next" ,
    "build" : " next build",
    "start" : "next start"
  },
```
4. 创建pages文件夹和文件
在根目录下，创建一个pages文件夹，这个文件夹是Next规定的，在这个文件夹下写入的文件，Next.js会自动创建对应的路由
有了文件夹以后，在文件下面创建一个index.js文件，这就是我们的首页了
简单的代码：
```
function Demo(){
    return (
        <div>Hello world</div>
    )
}
export default Demo
```
写好后在终端中使用 yarn dev 打开预览
二、快速创建Next.js项目
1. 安装creat-next-app
```
npm install -g create-next-app
```
2. 支持三种安装方式(npx、yarn、create-next-app)
以npx为例，三种安装方式安装的结构是一样
```
 npx creacte-next-app next-create
```
安装完以后执行 yarn dev 测试项目
在浏览器中输入http://localhost:3000,看到内容，说明项目生成成功