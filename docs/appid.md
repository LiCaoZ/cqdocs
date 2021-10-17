# AppID规范

`appid` 是应用的唯一标识符，形如 `com.example.music`。同一个应用的应用标识符长期不变，不同应用标识符不同。

应用开发过程中，相关文件存放于 `dev/[appid]/` 目录下。应用打包后，应用文件名为 `[appid].cpk`。

> **错误的 `appid` 会影响应用版权证明以及开发者权益，还有可能影响后续的发布、更新流程。**请阅读本文，为应用正确设置 `appid`。

### 格式 <a href="ge-shi" id="ge-shi"></a>

`appid` 的格式为 `域名反写`.`应用英文名`。

### 域名反写 <a href="yu-ming-fan-xie" id="yu-ming-fan-xie"></a>

开发者持有的域名的反写形式。可使用数字、**小写**字母、短横线(-)、点(.)。

**例如：**开发者的域名为：`example.com`，则**域名反写**则为 `com.example`（无需www）

> **注意：**开发者域名是指开发者（或团体）拥有**所有权**的域名（通常指在域名商购买，拥有完全的控制权限）。\
> 部分免费空间等附赠的域名可能功能受限（如无法设置 TXT 记录），使用此类域名可能会造成在证明应用版权中出现困难。

如果开发者没有或不便使用自己的域名，也可使用 酷Q 的开发者域名：`*.cqp.me`。

其中 `*` 代表开发者的英文名，由每位开发者自定义。为保证唯一性，该域名应未曾被其他开发者使用。

### 应用英文名 <a href="ying-yong-ying-wen-ming" id="ying-yong-ying-wen-ming"></a>

用于标识应用的英文名。可使用数字、**小写**字母、短横线(-)、下划线(\_)。

**例如：**weather、music、text2speech

### 例子 <a href="li-zi" id="li-zi"></a>

> 举例：有一款天气应用。\
> 开发者的域名为 `example.com`\
> 应用英文名为 `weather`\
> 则 appid 为 `com.example.weather`
>
> 举例：开发者的英文名为 Hanyuu\
> 开发者选取了域名 `hanyuu.cqp.me`\
> 应用英文名为 `weather`\
> 则 appid 为 `me.cqp.hanyuu.weather`\
>
