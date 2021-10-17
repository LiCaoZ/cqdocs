# CQ码

**CQ码**，是指在 酷Q 的消息中，以 `[CQ:` 开头、`]` 结尾的，可以实现特殊功能的代码。

**CQ码**，是指在 酷Q 的消息中，以 `[CQ:` 开头、`]` 结尾的，可以实现特殊功能的代码。

**CQ码**，是指在 酷Q 的消息中，以 `[CQ:` 开头、`]` 结尾的，可以实现特殊功能的代码。

### 结构 <a href="jie-gou" id="jie-gou"></a>

### 结构 <a href="jie-gou" id="jie-gou"></a>

CQ码的结构为 `[CQ:function,key=value,...]`

### 结构 <a href="jie-gou" id="jie-gou"></a>

其中 `function` 为功能名，`key` 为参数名，`value` 为参数值，`key=value` 称为一组参数。

CQ码的结构为 `[CQ:function,key=value,...]`

一个CQ码可以包含零组、一组或多组参数，功能名与每组参数之间用半角逗号 `,` 分割。

CQ码的结构为 `[CQ:function,key=value,...]`

### 规范 <a href="gui-fan" id="gui-fan"></a>

其中 `function` 为功能名，`key` 为参数名，`value` 为参数值，`key=value` 称为一组参数。

* CQ码是**大小写敏感**的，使用时请注意大小写。
*   对于不在CQ码内的消息（即文本消息），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    ```
* CQ码中的 `function`（功能名）与 `key`（参数名），仅支持大小写字母、数字、短横线（-）、下划线（\_）及点号（.）。
*   对于CQ码中的 `value`（参数值），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    , -> &#44;
    ```

其中 `function` 为功能名，`key` 为参数名，`value` 为参数值，`key=value` 称为一组参数。

### 目前支持的代码 <a href="mu-qian-zhi-chi-de-dai-ma" id="mu-qian-zhi-chi-de-dai-ma"></a>

一个CQ码可以包含零组、一组或多组参数，功能名与每组参数之间用半角逗号 `,` 分割。

#### 系统表情 <a href="xi-tong-biao-qing" id="xi-tong-biao-qing"></a>

一个CQ码可以包含零组、一组或多组参数，功能名与每组参数之间用半角逗号 `,` 分割。

```
[CQ:face,id={1}]
```

### 规范 <a href="gui-fan" id="gui-fan"></a>

`{1}` 为≥0的数字

### 规范 <a href="gui-fan" id="gui-fan"></a>

> **例子**\
> \[CQ:face,id=14]（发送一个微笑的系统表情）

* CQ码是**大小写敏感**的，使用时请注意大小写。
*   对于不在CQ码内的消息（即文本消息），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    ```
* CQ码中的 `function`（功能名）与 `key`（参数名），仅支持大小写字母、数字、短横线（-）、下划线（\_）及点号（.）。
*   对于CQ码中的 `value`（参数值），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    , -> &#44;
    ```
* CQ码是**大小写敏感**的，使用时请注意大小写。
*   对于不在CQ码内的消息（即文本消息），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    ```
* CQ码中的 `function`（功能名）与 `key`（参数名），仅支持大小写字母、数字、短横线（-）、下划线（\_）及点号（.）。
*   对于CQ码中的 `value`（参数值），为了防止解析混淆，需要进行**转义**。\
    转义规则如下：

    ```
    & -> &amp;
    [ -> &#91;
    ] -> &#93;
    , -> &#44;
    ```

#### emoji表情 <a href="emoji-biao-qing" id="emoji-biao-qing"></a>

### 目前支持的代码 <a href="mu-qian-zhi-chi-de-dai-ma" id="mu-qian-zhi-chi-de-dai-ma"></a>

```
[CQ:emoji,id={1}]
```

### 目前支持的代码 <a href="mu-qian-zhi-chi-de-dai-ma" id="mu-qian-zhi-chi-de-dai-ma"></a>

`{1}` emoji字符的unicode编号

#### 系统表情 <a href="xi-tong-biao-qing" id="xi-tong-biao-qing"></a>

> **例子**\
> \[CQ:emoji,id=128513]（发送一个大笑的emoji表情）

#### 系统表情 <a href="xi-tong-biao-qing" id="xi-tong-biao-qing"></a>

#### 原创表情 <a href="yuan-chuang-biao-qing" id="yuan-chuang-biao-qing"></a>

```
[CQ:face,id={1}]
```

```
[CQ:bface,id={1}]
```

```
[CQ:face,id={1}]
```

`{1}` 该原创表情的ID，存放在酷Q目录的data\bface\下

`{1}` 为≥0的数字

#### 小表情 <a href="xiao-biao-qing" id="xiao-biao-qing"></a>

`{1}` 为≥0的数字

```
[CQ:sface,id={1}]
```

> **例子**\
> \[CQ:face,id=14]（发送一个微笑的系统表情）

`{1}` 该小表情的ID

> **例子**\
> \[CQ:face,id=14]（发送一个微笑的系统表情）

#### 自定义图片 <a href="zi-ding-yi-tu-pian" id="zi-ding-yi-tu-pian"></a>

#### emoji表情 <a href="emoji-biao-qing" id="emoji-biao-qing"></a>

```
[CQ:image,file={1}]
```

#### emoji表情 <a href="emoji-biao-qing" id="emoji-biao-qing"></a>

`{1}` 图片文件名称，图片存放在酷Q目录的data\image\下

```
[CQ:emoji,id={1}]
```

> **例子**\
> \[CQ:image,file=1.jpg]（发送data\image\1.jpg）

```
[CQ:emoji,id={1}]
```

#### 语音 <a href="yu-yin" id="yu-yin"></a>

`{1}` emoji字符的unicode编号

```
[CQ:record,file={1},magic={2}]
```

`{1}` emoji字符的unicode编号

`{1}` 音频文件名称，音频存放在酷Q目录的data\record\下\
`{2}` 是否为变声，若该参数为**true**则显示变声标记。该参数可被忽略。

> **例子**\
> \[CQ:emoji,id=128513]（发送一个大笑的emoji表情）

> **例子**\
> \[CQ:record,file=1.silk,magic=true]（发送data\record\1.silk，并标记为变声）

> **例子**\
> \[CQ:emoji,id=128513]（发送一个大笑的emoji表情）

#### @某人 <a href="mou-ren" id="mou-ren"></a>

#### 原创表情 <a href="yuan-chuang-biao-qing" id="yuan-chuang-biao-qing"></a>

```
[CQ:at,qq={1}]
```

#### 原创表情 <a href="yuan-chuang-biao-qing" id="yuan-chuang-biao-qing"></a>

`{1}` 被@的群成员帐号。若该参数为**all**，则@全体成员（次数用尽或权限不足则会转换为文本）。

```
[CQ:bface,id={1}]
```

> **例子**\
> \[CQ:at,qq=123456]

```
[CQ:bface,id={1}]
```

#### 猜拳魔法表情 <a href="cai-quan-mo-fa-biao-qing" id="cai-quan-mo-fa-biao-qing"></a>

`{1}` 该原创表情的ID，存放在酷Q目录的data\bface\下

```
[CQ:rps,type={1}]
```

`{1}` 该原创表情的ID，存放在酷Q目录的data\bface\下

`{1}` 为猜拳结果的类型，暂不支持发送时自定义。该参数可被忽略。\
1 - 猜拳结果为石头\
2 - 猜拳结果为剪刀\
3 - 猜拳结果为布

#### 小表情 <a href="xiao-biao-qing" id="xiao-biao-qing"></a>

#### 掷骰子魔法表情 <a href="zhi-tou-zi-mo-fa-biao-qing" id="zhi-tou-zi-mo-fa-biao-qing"></a>

#### 小表情 <a href="xiao-biao-qing" id="xiao-biao-qing"></a>

```
[CQ:dice,type={1}]
```

```
[CQ:sface,id={1}]
```

`{1}` 对应掷出的点数，暂不支持发送时自定义。该参数可被忽略。

```
[CQ:sface,id={1}]
```

#### 戳一戳 <a href="chuo-yi-chuo" id="chuo-yi-chuo"></a>

`{1}` 该小表情的ID

```
[CQ:shake]
```

`{1}` 该小表情的ID

仅支持好友消息使用。

#### 自定义图片 <a href="zi-ding-yi-tu-pian" id="zi-ding-yi-tu-pian"></a>

#### 地点 <a href="di-dian" id="di-dian"></a>

#### 自定义图片 <a href="zi-ding-yi-tu-pian" id="zi-ding-yi-tu-pian"></a>

```
[CQ:location,lat={1},lon={2},title={3},content={4}]
```

```
[CQ:image,file={1}]
```

`{1}` 纬度\
`{2}` 经度\
`{3}` 分享地点的名称\
`{4}` 分享地点的具体地址

```
[CQ:image,file={1}]
```

> **例子**\
> \[CQ:location,lat=39.918056,lon=116.397027,title=故宫博物院,content=北京市东城区景山前街4号]

`{1}` 图片文件名称，图片存放在酷Q目录的data\image\下

#### 签到 <a href="qian-dao" id="qian-dao"></a>

`{1}` 图片文件名称，图片存放在酷Q目录的data\image\下

```
[CQ:sign,location={1},title={2},image={3}]
```

> **例子**\
> \[CQ:image,file=1.jpg]（发送data\image\1.jpg）

该CQ码仅支持接收。\
`{1}` 用户签到的地点，为中文字串\
`{2}` 用户签到时发表的心情文字\
`{3}` 签到卡片所使用的背景图片连接

> **例子**\
> \[CQ:image,file=1.jpg]（发送data\image\1.jpg）

#### 音乐 <a href="yin-le" id="yin-le"></a>

#### 语音 <a href="yu-yin" id="yu-yin"></a>

```
[CQ:music,type={1},id={2},style={3}]
```

#### 语音 <a href="yu-yin" id="yu-yin"></a>

`{1}` 音乐平台类型，目前支持qq、163\
`{2}` 对应音乐平台的数字音乐id\
`{3}` 音乐卡片的风格。仅 Pro 支持该参数，该参数可被忽略。

```
[CQ:record,file={1},magic={2}]
```

> **例子**\
> \[CQ:music,type=qq,id=422594]（发送一首QQ音乐的“Time after time”歌曲到群内）\
> \[CQ:music,type=163,id=28406557]（发送一首网易云音乐的“桜咲く”歌曲到群内）

```
[CQ:record,file={1},magic={2}]
```

#### 音乐自定义分享 <a href="yin-le-zi-ding-yi-fen-xiang" id="yin-le-zi-ding-yi-fen-xiang"></a>

`{1}` 音频文件名称，音频存放在酷Q目录的data\record\下\
`{2}` 是否为变声，若该参数为**true**则显示变声标记。该参数可被忽略。

```
[CQ:music,type=custom,url={1},audio={2},title={3},content={4},image={5}]
```

`{1}` 音频文件名称，音频存放在酷Q目录的data\record\下\
`{2}` 是否为变声，若该参数为**true**则显示变声标记。该参数可被忽略。

`{1}` 分享链接，即点击分享后进入的音乐页面（如歌曲介绍页）。\
`{2}` 音频链接（如mp3链接）。\
`{3}` 音乐的标题，建议12字以内。\
`{4}` 音乐的简介，建议30字以内。该参数可被忽略。\
`{5}` 音乐的封面图片链接。若参数为空或被忽略，则显示默认图片。

> **例子**\
> \[CQ:record,file=1.silk,magic=true]（发送data\record\1.silk，并标记为变声）

#### 链接分享 <a href="lian-jie-fen-xiang" id="lian-jie-fen-xiang"></a>

> **例子**\
> \[CQ:record,file=1.silk,magic=true]（发送data\record\1.silk，并标记为变声）

```
[CQ:share,url={1},title={2},content={3},image={4}]
```

#### @某人 <a href="mou-ren" id="mou-ren"></a>

`{1}` 分享链接。\
`{2}` 分享的标题，建议12字以内。\
`{3}` 分享的简介，建议30字以内。该参数可被忽略。\
`{4}` 分享的图片链接。若参数为空或被忽略，则显示默认图片。

#### @某人 <a href="mou-ren" id="mou-ren"></a>

```
[CQ:at,qq={1}]
```

```
[CQ:at,qq={1}]
```

`{1}` 被@的群成员帐号。若该参数为**all**，则@全体成员（次数用尽或权限不足则会转换为文本）。

`{1}` 被@的群成员帐号。若该参数为**all**，则@全体成员（次数用尽或权限不足则会转换为文本）。

> **例子**\
> \[CQ:at,qq=123456]

> **例子**\
> \[CQ:at,qq=123456]

#### 猜拳魔法表情 <a href="cai-quan-mo-fa-biao-qing" id="cai-quan-mo-fa-biao-qing"></a>

#### 猜拳魔法表情 <a href="cai-quan-mo-fa-biao-qing" id="cai-quan-mo-fa-biao-qing"></a>

```
[CQ:rps,type={1}]
```

```
[CQ:rps,type={1}]
```

`{1}` 为猜拳结果的类型，暂不支持发送时自定义。该参数可被忽略。\
1 - 猜拳结果为石头\
2 - 猜拳结果为剪刀\
3 - 猜拳结果为布

`{1}` 为猜拳结果的类型，暂不支持发送时自定义。该参数可被忽略。\
1 - 猜拳结果为石头\
2 - 猜拳结果为剪刀\
3 - 猜拳结果为布

#### 掷骰子魔法表情 <a href="zhi-tou-zi-mo-fa-biao-qing" id="zhi-tou-zi-mo-fa-biao-qing"></a>

#### 掷骰子魔法表情 <a href="zhi-tou-zi-mo-fa-biao-qing" id="zhi-tou-zi-mo-fa-biao-qing"></a>

```
[CQ:dice,type={1}]
```

```
[CQ:dice,type={1}]
```

`{1}` 对应掷出的点数，暂不支持发送时自定义。该参数可被忽略。

`{1}` 对应掷出的点数，暂不支持发送时自定义。该参数可被忽略。

#### 戳一戳 <a href="chuo-yi-chuo" id="chuo-yi-chuo"></a>

#### 戳一戳 <a href="chuo-yi-chuo" id="chuo-yi-chuo"></a>

```
[CQ:shake]
```

```
[CQ:shake]
```

仅支持好友消息使用。

仅支持好友消息使用。

#### 地点 <a href="di-dian" id="di-dian"></a>

#### 地点 <a href="di-dian" id="di-dian"></a>

```
[CQ:location,lat={1},lon={2},title={3},content={4}]
```

```
[CQ:location,lat={1},lon={2},title={3},content={4}]
```

`{1}` 纬度\
`{2}` 经度\
`{3}` 分享地点的名称\
`{4}` 分享地点的具体地址

`{1}` 纬度\
`{2}` 经度\
`{3}` 分享地点的名称\
`{4}` 分享地点的具体地址

> **例子**\
> \[CQ:location,lat=39.918056,lon=116.397027,title=故宫博物院,content=北京市东城区景山前街4号]

> **例子**\
> \[CQ:location,lat=39.918056,lon=116.397027,title=故宫博物院,content=北京市东城区景山前街4号]

#### 签到 <a href="qian-dao" id="qian-dao"></a>

#### 签到 <a href="qian-dao" id="qian-dao"></a>

```
[CQ:sign,location={1},title={2},image={3}]
```

```
[CQ:sign,location={1},title={2},image={3}]
```

该CQ码仅支持接收。\
`{1}` 用户签到的地点，为中文字串\
`{2}` 用户签到时发表的心情文字\
`{3}` 签到卡片所使用的背景图片连接

该CQ码仅支持接收。\
`{1}` 用户签到的地点，为中文字串\
`{2}` 用户签到时发表的心情文字\
`{3}` 签到卡片所使用的背景图片连接

#### 音乐 <a href="yin-le" id="yin-le"></a>

#### 音乐 <a href="yin-le" id="yin-le"></a>

```
[CQ:music,type={1},id={2},style={3}]
```

```
[CQ:music,type={1},id={2},style={3}]
```

`{1}` 音乐平台类型，目前支持qq、163\
`{2}` 对应音乐平台的数字音乐id\
`{3}` 音乐卡片的风格。仅 Pro 支持该参数，该参数可被忽略。

`{1}` 音乐平台类型，目前支持qq、163\
`{2}` 对应音乐平台的数字音乐id\
`{3}` 音乐卡片的风格。仅 Pro 支持该参数，该参数可被忽略。

> **例子**\
> \[CQ:music,type=qq,id=422594]（发送一首QQ音乐的“Time after time”歌曲到群内）\
> \[CQ:music,type=163,id=28406557]（发送一首网易云音乐的“桜咲く”歌曲到群内）

> **例子**\
> \[CQ:music,type=qq,id=422594]（发送一首QQ音乐的“Time after time”歌曲到群内）\
> \[CQ:music,type=163,id=28406557]（发送一首网易云音乐的“桜咲く”歌曲到群内）

#### 音乐自定义分享 <a href="yin-le-zi-ding-yi-fen-xiang" id="yin-le-zi-ding-yi-fen-xiang"></a>

#### 音乐自定义分享 <a href="yin-le-zi-ding-yi-fen-xiang" id="yin-le-zi-ding-yi-fen-xiang"></a>

```
[CQ:music,type=custom,url={1},audio={2},title={3},content={4},image={5}]
```

```
[CQ:music,type=custom,url={1},audio={2},title={3},content={4},image={5}]
```

`{1}` 分享链接，即点击分享后进入的音乐页面（如歌曲介绍页）。\
`{2}` 音频链接（如mp3链接）。\
`{3}` 音乐的标题，建议12字以内。\
`{4}` 音乐的简介，建议30字以内。该参数可被忽略。\
`{5}` 音乐的封面图片链接。若参数为空或被忽略，则显示默认图片。

`{1}` 分享链接，即点击分享后进入的音乐页面（如歌曲介绍页）。\
`{2}` 音频链接（如mp3链接）。\
`{3}` 音乐的标题，建议12字以内。\
`{4}` 音乐的简介，建议30字以内。该参数可被忽略。\
`{5}` 音乐的封面图片链接。若参数为空或被忽略，则显示默认图片。

#### 链接分享 <a href="lian-jie-fen-xiang" id="lian-jie-fen-xiang"></a>

#### 链接分享 <a href="lian-jie-fen-xiang" id="lian-jie-fen-xiang"></a>

```
[CQ:share,url={1},title={2},content={3},image={4}]
```

```
[CQ:share,url={1},title={2},content={3},image={4}]
```

`{1}` 分享链接。\
`{2}` 分享的标题，建议12字以内。\
`{3}` 分享的简介，建议30字以内。该参数可被忽略。\
`{4}` 分享的图片链接。若参数为空或被忽略，则显示默认图片。

`{1}` 分享链接。\
`{2}` 分享的标题，建议12字以内。\
`{3}` 分享的简介，建议30字以内。该参数可被忽略。\
`{4}` 分享的图片链接。若参数为空或被忽略，则显示默认图片。
