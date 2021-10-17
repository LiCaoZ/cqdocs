# 开发模式

**开发模式**，是为了便于开发者开发的需求，在酷Q中内置的一系列功能。

可以通过编辑 `conf/CQP.cfg` 来开启及关闭这些调试功能。

### 快速开启（推荐） <a href="kuai-su-kai-qi-tui-jian" id="kuai-su-kai-qi-tui-jian"></a>

您可以通过高级设置窗口快速开启**开发模式**。操作步骤：

1. 悬浮窗右键 > 应用 > 应用管理，打开**应用**窗口
2. 左键连续点击应用窗口右下角的版本号**5次**
3. 在弹出的高级设置窗口中即可开启开发模式

![](https://docs.cqp.im/img/dev-enable.png)

### 通过配置文件设置﻿ <a href="tong-guo-pei-zhi-wen-jian-she-zhi" id="tong-guo-pei-zhi-wen-jian-she-zhi"></a>

**您也可以手动编辑配置文件开启开发模式。**

打开 酷Q 目录下的 `conf/CQP.cfg` 文件，并在文件末尾插入以下一行（如已有本行需跳过此步）。

* 您可以使用“Visual Studio Code”、“记事本”等文本编辑器编辑本文件。
* 如果本文件不存在，您可以先启动一次 酷Q，本文件将自动被生成。

在文件中，添加

```
[Dev]  
Enable=1
```

并重启，即可开启开发模式。
