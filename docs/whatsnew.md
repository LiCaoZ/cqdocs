# 新特性

在 酷Q 的 **V9应用机制** 中，引入了许多新的特性，并着重优化了开发者体验，使应用更安全、自由。

您可以将旧版机制的应用升级至 V9，参见[V8更新至V9](https://docs.cqp.im/dev/upgrade/v8-v9/)。

### 开发模式 <a href="kai-fa-mo-shi" id="kai-fa-mo-shi"></a>

开发者在**开发模式**下可以更便捷地开发应用，参见[开启开发模式](https://docs.cqp.im/dev/v9/devmode/)。

### 打包机制 <a href="da-bao-ji-zhi" id="da-bao-ji-zhi"></a>

V9中引入了**打包机制**，将常量中的应用信息放到了单独的文件 `app.json` 中（打包时会重新并入cpk）。

这带来了以下好处：

* 酷Q启动时，dll/cpk 不会再占用，可以随时替换（重载生效）。
* 酷Q启动时，可以直接编辑 `app.json`（重载生效）。
* 打包后的 `app.cpk` 经过压缩、加密，安全性较高。

### 好友、临时消息合并 <a href="hao-you-lin-shi-xiao-xi-he-bing" id="hao-you-lin-shi-xiao-xi-he-bing"></a>

好友（Type=1）、临时（Type=3）消息已经**合并**为私聊（Type=21）消息，并且前两者在V9中已经停用。同时，发送私聊消息的Api也已经统一。省去了区分好友消息、临时消息时的烦恼。

### 消息支持正则过滤 <a href="xiao-xi-zhi-chi-zheng-ze-guo-lv" id="xiao-xi-zhi-chi-zheng-ze-guo-lv"></a>

使用正则过滤，可以方便用户自定义命令，并且方便提取命令。

### 新的开发流程 <a href="xin-de-kai-fa-liu-cheng" id="xin-de-kai-fa-liu-cheng"></a>

1. [开启开发模式](https://docs.cqp.im/dev/v9/devmode/)
2. 应用保存为 `app.dll`，应用信息保存为 `app.json`。在应用列表可以直接加载。
3. 成功加载后，可以测试应用，或者在应用窗口打包。
4. 打包完毕的应用可以直接发布。

具体流程可以浏览[快速入门指南](https://docs.cqp.im/dev/v9/getting-started/)。
