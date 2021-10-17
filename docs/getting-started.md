# 快速入门

**欢迎参与 酷Q 应用开发！**

在本指南中，您将了解 酷Q V9 应用的开发方式，并开发出一个简单的复读应用。

### 获取SDK <a href="huo-qu-sdk" id="huo-qu-sdk"></a>

您可以在 酷Q社区 获取 酷Q 的 **SDK**（软件开发工具包）。

> 地址：[https://cqp.cc/t/15124](https://cqp.cc/t/15124)

> 本文档主要介绍了 **易语言 SDK** 的快速入门，其他语言的开发可以浏览相应代码库（文档）。

### 开始之前.. <a href="kai-shi-zhi-qian" id="kai-shi-zhi-qian"></a>

#### 开启开发模式 <a href="kai-qi-kai-fa-mo-shi" id="kai-qi-kai-fa-mo-shi"></a>

![](https://docs.cqp.im/img/dev-enable.png)

步骤：悬浮窗右键 > 应用 > 应用管理，左键点击应用窗口右下角版本号**5次**，在弹出的窗口中开启开发模式并重启。

开启开发模式后，酷Q将新增以下功能，帮助您进行开发：

* 错误信息将详细显示。
* 支持载入、打包未打包应用。（开启开发模式后才能载入开发中的应用）
* 在应用窗口，按住shift并单击“重启酷Q”，可以快速重载应用（而无需重启）。

### 简单编译范例SDK <a href="jian-dan-bian-yi-fan-li-sdk" id="jian-dan-bian-yi-fan-li-sdk"></a>

解压下载到的SDK（如 **CQP_SDK_V9\_XXXXXX.zip**），并打开SDK目录。

其中以`CQP_EL`开头的目录为 **易语言 SDK**。

#### 易语言 SDK <a href="yi-yu-yan-sdk" id="yi-yu-yan-sdk"></a>

1. 阅读 易语言SDK说明.txt，了解各文件的用途。
2. 将 `com.example.demo` 目录复制到酷Q的 `dev` 目录下（开启开发模式后，会自动创建 `dev` 目录）。
3. 使用已经配置完毕（支持**静态编译**）的易语言，打开 `dev/com.example.demo/app.e`。
4. 在 `_eventPrivateMsg`、`_eventGroupMsg` 子程序下，已经包含了一些测试语句（用于自动回复私聊消息、群消息）。
   * 您可以试着猜测这些测试语句的效果，也可以尝试改动这些测试语句，看看编译后会有什么不同的效果。
   * 打开日志窗（悬浮窗右键 > 日志），看看酷Q是如何接收、发送消息的。
   * 推荐使用专用机器人帐号（如果还没有，不妨申请一个），私聊/单独开群组做测试，测试的时候不要打扰到群友哦\~
5. 点击易语言IDE上的**编译 > 静态编译**，将编译出的dll文件放在 `dev/com.example.demo/app.dll`。
6. 确认 `dev/com.example.demo/app.json` 已经存在。
   * 您可以将酷Q的 `dev/[appid]` 目录作为您的工作目录。
7. 启动酷Q，悬浮窗右键 > 应用 > 应用目录 > 应用管理，您所编译的应用应该已经出现在了应用列表内！

### 设置 `appid` <a href="she-zhi-appid" id="she-zhi-appid"></a>

`appid` 是应用的唯一标识符。同一个应用的应用标识符长期不变，不同应用标识符不同，参见 [appid 规则](https://docs.cqp.im/dev/v9/appid/)。

确定该应用的 `appid` 后，请将应用目录名 `com.example.demo` 改为您设置的 `appid`。

> **错误的 `appid` 会影响应用版权证明以及开发者权益，还有可能影响后续的发布、更新流程。**请阅读 [appid 规则](https://docs.cqp.im/dev/v9/appid/)，为应用正确设置 `appid`。

### 打包应用 <a href="da-bao-ying-yong" id="da-bao-ying-yong"></a>

开发完成后，您可以打包应用，将应用与他人分享。

1.  阅读 [app.json](https://docs.cqp.im/dev/v9/app.json/)，编辑应用的 .json 文件及 .dll 的文件名，修改 appid、应用名称、作者等信息。

    > **错误的信息或将影响您的开发者权益**，请阅读 [app.json](https://docs.cqp.im/dev/v9/app.json/)，正确设置应用基础信息。
2. 在 .json 文件中，移除不必要的菜单、权限。
3. 启动酷Q，悬浮窗右键 > 应用 > 应用目录 > 应用管理，选中你的应用，点击右下角的开发按钮，选择打包。
4. 将生成的 cpk 文件发布到 [应用发布](https://cqp.cc/b/app) 板块，在社区分享您开发的应用吧！

欢迎加入**开发交流群**（群号：325405886），与更多开发者共同交流、探讨。
