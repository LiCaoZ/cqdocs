# event(事件)

`event`，是指标识**应用所需接收的事件**的信息。在 `app.json` 文件中定义。

> 为使开发更加便捷，请按照实际需求，合理选择需要的事件，并选用恰当的参数。

### 用途 <a href="yong-tu" id="yong-tu"></a>

在酷Q运行过程中，有许多**事务**（如收到一条新消息等）需要交给应用来处理。而**事件**(**event**)就是将这些**事务**传递给应用的桥梁。

每个应用可以在 `app.json` 的 `event` 部分中申请接收多种类型的事件，用于处理不同方面的**事务**。

> 同一个事件可以申请多次，并使用不同的 `id` 及 `function` 区分。

### 参数 <a href="can-shu" id="can-shu"></a>

#### `id` <a href="id" id="id"></a>

**事件唯一ID**，整数，每个整数对应唯一的事件。这意味着您将可以使同一事件类型对应多个事件。

#### `name` <a href="name" id="name"></a>

**事件名称**，字符串，该参数将显示于事件列表中以便用户调整事件优先级等。

#### `type` <a href="type" id="type"></a>

**事件类型**，整数，每个整数代表一种事件类型。

#### `name` <a href="name-1" id="name-1"></a>

**事件名称**，字符串，如“好友消息处理”等，将在酷Q应用的事件列表中显示，供用户区分。

#### `function` <a href="function" id="function"></a>

**事件对应函数**，字符串，用于指定接收事件的函数。

根据 `type`（事件类型）的不同，该函数所需要的参数以及接收到的事件也会有所不同。

#### `priority` <a href="priority" id="priority"></a>

**优先级**，整数，数值越大，优先级越低。

目前支持以下四种优先级：

* **10000** 最高 - 监控类应用，无法用于拦截消息。（如：消息数目统计等）
* **20000** 高 - 消息控制类应用，可用于拦截消息。（如：机器人开关等）
* **30000** 一般 - 普通功能类应用。（如：天气查询、游戏类等）
* **40000** 低 - 聊天对话类应用。（如：词库、云词库）

请按照实际需求选择优先级。如果同一个事件需要应对多种不同优先级的功能，可以申请多个事件，并使用不同的`function`（事件对应函数）及`priority`（优先级）。

#### `regex` <a href="regex" id="regex"></a>

**消息的正则表达式滤器**，具体示例可见官方 SDK。本参数可选。