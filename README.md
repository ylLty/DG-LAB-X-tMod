![icon](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/icon.png?raw=true)

# DG-LAB X tMod

将泰拉瑞亚与DG-LAB连接起来。当游戏人物受伤害时，现实中的你也会被电！

> Copyright (C) 2025 yl_lty
>
> DGLAB是本模组的简称（仅在泰拉瑞亚话题或语境中）

## 声明

- 使用该模组前，请**务必阅读此文档**。

- **未成年人严禁使用此软件**，请未成年玩家自觉禁用此模组。

- 本模组内置安全确认功能以确保合规使用，开发者鼓励用户根据MIT协议自由修改和分发代码，**但提醒移除安全机制可能违反当地法律甚至导致人身风险。**

- **禁止在使用此模组时直播**，若因违规使用该模组受到直播间封禁或账号封禁等处罚措施，责任不由开发者承担。

- **不得将此模组用于任何非法用途。**

- 务必**阅读并遵守DG-LAB安全须知**，安全须知内容如图：

  ![安全须知](https://raw.githubusercontent.com/ylLty/DG-LAB-X-tMod/refs/heads/main/DGLAB%E6%89%8B%E5%86%8C%E6%89%AB%E6%8F%8F%E4%BB%B6%EF%BC%88%E4%BE%B5%E5%88%A0%EF%BC%89/1%E5%AE%89%E5%85%A8%E9%A1%BB%E7%9F%A5.webp)

## 使用方式

考虑到玩郊狼的大多数人都会搞计算机，所以这个文档写的不会很详细，请见谅。~~疑似祖师爷的诅咒（~~

> 我知道图灵只是个0，不要太较真哈

### 1、下载

1、在 Steam 创意工坊中，订阅模组“[DG-LAB X tMod](https://steamcommunity.com/sharedfiles/filedetails/?id=3542577337)”~~这一块~~

2、待到安装完成后，启动游戏

### 2、配置

1、在游戏主菜单中依次点击 创意工坊-管理模组-模组配置-“DG-LAB X tMod”-客户端配置

2、**阅读并确认重要安全警示。**

3、根据提示自行修改配置内容（可选）

波形要求:

*（请不要在C:\Users\Administrator\Documents\My Games\Terraria\tModLoader\ModConfigs\DGLABtMod_MainConfig.json当中进行修改）*

如图

![ConfigExample](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/ConfigExample.png?raw=true)

### 连接

1、玩家进入世界后，屏幕上方会出现一个强度显示面板（看不见可以试试全屏）

如图

![UIExam](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/UIExam.png?raw=true)

2、按照提示，鼠标右键点击强度显示面板进行连接

3、此时会自动使用系统默认图片浏览器打开二维码图片。点击DG-LAB应用首页中的 SOCKET控制，在点击 连接SOCKET服务，扫描刚刚打开的二维码就可以了

> 如果遇到问题，请在 已知问题 处寻找解决方法

祝您玩得愉快! ヾ(≧▽≦*)o



## 已知问题

### 1、无法启动服务

一般来说，如果遇到以下几种提示，可以**试试在配置页面修改端口号**：

![port1](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E5%B7%B2%E7%9F%A5%E9%97%AE%E9%A2%98%E5%9B%BE%E7%89%87/%E7%AB%AF%E5%8F%A3%E5%8D%A0%E7%94%A8%E4%B9%8B%E4%B8%80.png?raw=true)

![port2](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E5%B7%B2%E7%9F%A5%E9%97%AE%E9%A2%98%E5%9B%BE%E7%89%87/%E7%AB%AF%E5%8F%A3%E5%8D%A0%E7%94%A8%E4%B9%8B%E4%BA%8C.png?raw=true)

如果不行，可以**尝试重启软件**，某些情况下，可能还需要**检查防火墙**

> 其他的无法启动我暂时没有遇到过

### 2、无法连接SOCKET服务

由于SOCKET服务运行在玩家电脑本地，依靠局域网与手机连接。**所以请保持手机与电脑连接同一个WLAN，且确保网络没有隔离**

如果还是没有效果，可以**在[草料二维码解码器](https://cli.im/deqr)中解析生成的连接二维码，并确认二维码文本内容中`192.168.1.1`与你的电脑IP一致**（可以在路由器管理页面确认）

二维码内容：

`https://www.dungeon-lab.com/app-download.php#DGLAB-SOCKET#ws://192.168.1.1:9999/kundusi0-xila-er0i-s0a0-bitch0dog012`

如果仍然不行，**请在cmd当中输入**`netstat -ano|Find "你设置的端口号"`

如果什么都没有输出，说明服务没有启动成功，**请尝试重启服务或者游戏**

如果输出  `TCP    0.0.0.0:你设置的端口号           0.0.0.0:0              LISTENING       20652`这样的文本，说明服务启动成功（？），那就是疑难杂症了，**试试重启电脑（？）**

#### 手机端卡在"正在连接"

这种情况可以**尝试先关闭App，然后重新打开App扫码**

### 3、关闭服务时卡死

尝试关闭服务时突然卡死，请不要慌张，**等一会就好了**

如果出现这样的提示（如图），说明服务器是已经关闭了的，忽略即可（原因未知，如有大佬指出，必将感谢）

![StopServer](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E5%B7%B2%E7%9F%A5%E9%97%AE%E9%A2%98%E5%9B%BE%E7%89%87/%E5%85%B3%E9%97%AD%E6%9C%8D%E5%8A%A1.png?raw=true)

### 4、时不时会报错

因为一些我还没有搞懂的原因，**有时**在tModLoader当中try{}catch{}并不会走到catch里面，还会在游戏里给橙色报错，这种**忽略即可**（？）

![ErrorExam](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E5%B7%B2%E7%9F%A5%E9%97%AE%E9%A2%98%E5%9B%BE%E7%89%87/%E6%97%A0%E4%BC%A4%E5%A4%A7%E9%9B%85.png?raw=true)

问题代码：

```c#
protected override void OnMessage(MessageEventArgs e)//处理来自 App 的消息的
{
    string message;
    string clientId;
    string targetId;
    string type;
    string relationsSize;
    string time;
    string channel;
    try
    {
        dynamic data = JsonConvert.DeserializeObject(e.Data);

        message = data.message;
        clientId = data.clientId;
        targetId = data.targetId;
        type = data.type;
        relationsSize = data.relationsSize;
        time = data.time;
        channel = data.channel;
    }//反序列化消息
    catch 
    {
        Main.NewText("消息解析失败",255);//根本走不到这里，但其他地方倒是没问题
        return; 
    }
}
```



## 其他说明

### 开源代码许可

1、QRCoder 1.6.0 : Copyright (c) 2013-2018 Raffael Herrmann

2、WebSocketSharp : Copyright (c) 2010-2025 sta.blockhead

### 其他

- 本模组部分代码由DeepSeek生成，同时部分代码也由Copilot生成。
- 本模组WebSocket服务部分参照了[此文本](https://github.com/DG-LAB-OPENSOURCE/DG-LAB-OPENSOURCE/blob/main/socket/BackEnd(Node)/websocketNode.js)。
- 本模组内置安全确认功能以确保合规使用，开发者鼓励用户根据MIT协议自由修改和分发代码，**但提醒移除安全机制可能违反当地法律甚至导致人身风险。**
- 用户本模组配置页面确认警告后方可使用
- DG-LAB官方已对DG-LAB 3.0设备输出进行了软硬件多重限制同时进行了安全警告，官方也已说明产品最高输出低于安全标准的限制。此模组也对强度大小进行了默认限制（为官方最大限制的50%）
- 本模组使用MIT协议。
### 赞助开发者Donate the Dev

喜欢本模组可以赞助支持！（下方查看二维码）

请备注`赞助DG-LAB X tMod - [你的github ID]`。所有赞助名单都将公布！(没有Github账号可以填写昵称)

若你想匿名赞助，请填写备注`赞助DG-LAB X tMod`但不备注你的信息，**否则我无法判断收款码收款意图！将不会纳入赞助名单！**

**暂不支持退款**。

[查看赞助名单](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E8%B5%9E%E5%8A%A9%E5%90%8D%E5%8D%95.md)


![Donate](https://github.com/ylLty/DG-LAB-X-tMod/blob/main/%E8%B5%9E%E5%8A%A9Donate.jpg?raw=true)

