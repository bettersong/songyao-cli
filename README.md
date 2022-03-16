# songyao-cli
文档地址：https://www.cnblogs.com/songyao666/p/11847754.html
#### 自研脚手架
全局安装
(注意这里镜像切到npm哦，其他镜像可能同步没这么快，之前自己也踩了这个坑，用了自己公司的镜像发现安装不上。)
```
npm i songyao-cli -g
```


检测是否已经全局安装
检测自己是否全局安装直接在终端输入sy,如有提示则说明安装成功了，或输入 sy -V,能出来版本号

查看当前版本支持的项目

```shell
sy list
```


你会看到当前1.1.3版本支持vue2,react,vue3,koa项目

初始化一个项目试试吧

```shell
sy init 模版名称 项目名称
```

**以vue为例**

输入`sy init sy-vue myPro`回车，这样就会帮你生成一个项目名为myPro的vue项目

注意sy-vue这是模板名，是固定的，表示生成vue项目，myPro这是项目名，可以自己任意修改

初始化完成是这样的（比较快，因为我并没有把依赖也一起初始化，所以下面在启动项目前，先要安装依赖，这是与其他框架提供的脚手架的不同之处，节省项目初始化时间）

启动项目（先安装依赖，再启动）
```
npm i ## 安装依赖
npm run serve ## 启动项目
```
