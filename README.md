# songyao-cli

![image-20220316151730931](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2b71L5t7aiaiaoxZxEhzY6EDkRuauc822EyLUUmJKuGxTaYziaianTFvQCQ/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

## 使用文档

### 全局安装

```shell
npm i songyao-cli -g
```

(注意这里镜像切到npm哦，其他镜像可能同步没这么快，之前自己也踩了这个坑，用了自己公司的镜像发现安装不上。)

### 检测安装是否成功

检测自己是否全局安装直接在终端输入sy,如过能看到下面的内容则说明脚手架安装成功了

```shell
sy
```

![image-20220316161603106](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe27EfFX94YicRr7jJvibT3QlNKHT6WUzWLSSicTwO4lIL79N8FFlxiabDibwQ/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

### 查看版本

```shell
sy -V
```

![image-20220316161700828](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2icVOUYMa34NKdiah9yicbNT2GV4EIT2KTXm5WmkfbfOnrQOqoKp2pOUaQ/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

### 查看当前版本支持的项目

```shell
sy list
```

![image-20220316161826435](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2UhUiaN6N06CWk1G6JicaJuCbvmMOZd11PCr6dTvYn2L2Ir2oEgeGGwxA/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

你会看到当前版本支持`vue2`、`react`、`vue3`、`koa`项目

### 初始化一个项目试试吧（以vue3为例）

```shell
sy init sy-vue@3 myVue3Test

## sy-vue@3 是你想要初始化的项目模版（对应sy list 中的模版key)
## myVue3Test 这个是你想要命名的项目名称（可自行定义）
```

![image-20220316165658413](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2FKpdNwrd4Yibocic8n2XyWVB0lQr2UVNPgN9jykPiaqTdnR3QGhoj2G6Q/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

然后再进入项目安装依赖

```shell
## 安装依赖
npm i 
```

![image-20220316170834429](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2BLzpVKGLX4YSd1WpPfuP4aSdiafhqVJHl4xO8V00o0fKIMzIW3sAabw/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

最后启动项目（启动命令到package.json中查找，每个项目可能不一样）

```shell
npm run dev
```

启动完你就能够看到下面这个页面

![image-20220316170112482](https://mmbiz.qpic.cn/mmbiz_png/aw5KtMic7pia5W36gzhX7wicOUZHa6mXKe2mXl1CbCNdgzsFdicDcibwkDRmv30QlmgPkHWtNsGk0QuicFwJbZvibmjxA/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)

到这里一个vue3+vite的项目就初始化好了，项目内默认已经配置好了eslint。

初始化其它项目与这个类似，只需选择好对应的模板初始化，然后再安装依赖就OK了。

## 最后

觉得不错的话，给作者点个star✨吧，如果你有什么需要的项目模版欢迎找我添加~
