# Dream-Msg

## 一款简约的基于原生 Javascript 的消息提示插件（带错误提示音）

> 一款简约的基于原生 Javascript 的消息提示插件（带错误提示音）。包含功能，`函数回调`，`自动关闭` ，`手动关闭` ，`错误提示音`，`loading`，`closeAll`等。


## 效果截图

<img src="./lib/screenshot.png" width="100%" />

## 使用说明

```html
 <script src="https://cdn.jsdelivr.net/gh/iGaoWei/Dream-Msg/lib/dream-msg.min.js"></script>
```

**info**

```js
// 默认
Dreamer.info("您有一条新消息待处理，请及时查收！");

//函数回调
Dreamer.info("您有一条新消息待处理，请及时查收！",function () {
    alert("我是自定义事件");
});

//手动关闭
Dreamer.info("您有一条新消息待处理，请及时查收！",0);

//自动关闭
Dreamer.info("您有一条新消息待处理，请及时查收！",2000);

//提示音
Dreamer.info("您有一条新消息待处理，请及时查收！",true);
```

**success**

```js
// 默认
Dreamer.success("密码修改成功请重新登录！");

//函数回调
Dreamer.success("密码修改成功请重新登录！",function () {
    alert("我是自定义事件");
});

//手动关闭
Dreamer.success("密码修改成功请重新登录！",0);

//自动关闭
Dreamer.success("密码修改成功请重新登录！",2000);

//提示音
Dreamer.success("密码修改成功请重新登录！",true);
```

**warning**

```js
// 默认
Dreamer.warning("系统异常这是一条警告信息！");

//函数回调
Dreamer.warning("系统异常这是一条警告信息！",function () {
    alert("我是自定义事件");
});

//手动关闭
Dreamer.warning("系统异常这是一条警告信息！",0);

//自动关闭
Dreamer.warning("系统异常这是一条警告信息！",2000);

//提示音
Dreamer.warning("系统异常这是一条警告信息！",true);
```

**error**

```js
// 默认
Dreamer.error("添加失败，请稍后再试！");

//函数回调
Dreamer.error("添加失败，请稍后再试！",function () {
    alert("我是自定义事件");
});

//手动关闭
Dreamer.error("添加失败，请稍后再试！",0);

//自动关闭
Dreamer.error("添加失败，请稍后再试！",2000);

//提示音
Dreamer.error("添加失败，请稍后再试！",true);
```

**loading**

```js
// 默认
Dreamer.loading("加载中，请稍后")

//自动关闭
var closeMsg = Dreamer.loading("加载中，请稍后");
setTimeout(function(){
    closeMsg();
}, 4000);
```

**closeAll**

```js
Dreamer.destroyAll();
```
