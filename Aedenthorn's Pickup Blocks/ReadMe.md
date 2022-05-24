# 注意！

由于本补丁面向的模组性质特殊，**本补丁的安装亦有较大区别**。

由`Aedenthron`创作的`Pickup Blocks`模组是一个程序注入型模组，使用`PickupBlocks.dll`为游戏植入了可拾起各种物块的功能。模组中不包括一般模组中用于提供文本和多语言支持的`Localization.txt`文件。幸而作者慷慨地将相关文本整合在了模组自有的设置文档内，因此将其中文化仍然可行。

## 安装步骤

* 首先，您仍然必须在模组的[发布页面](https://www.nexusmods.com/7daystodie/mods/2229)下载模组本体（戳左边的“发布页面”四个大字前往发布页）。
* 将您其解压缩至一个单独的目录内。
* 清理嵌套的目录，**您将要在之后的步骤中复制的目录应当直接包含且仅包含`ModInfo.xml`文件以及`PickupBlocks.dll`文件**。
* 将之前步骤中准备完成的目录直接复制到`[您的《7日杀》游戏根目录]\Mods\`目录下。
* 此模组需要在启动游戏时将`Easy Anti Cheat`功能关闭。您可以在游戏启动器中将与之对应的选项取消勾选。如果您是Steam用户，这需要您在Steam主程序中选择启动《7日杀》游戏，并选择`Show Game Launcher`选项。
* 打开此模组文件夹中的`ModInfo.xml`文件，比对模组版本（看`<Version value="此处为版本号" />`这一行）与本补丁兼容的模组版本（目前兼容版本为`0.1.0`），确保两者相符。如果两者不相符，请开个 issue 通知我。
* 确保版本相符后，将本文件夹内的`config.json`文件直接复制到模组文件夹内。
* 用记事本程序（或者其他您喜欢的文本编辑器）打开`config.json`文件，并根据您的喜好编辑模组的设置（相关内容请见下一段内容）。
* 
## 模组设置文件详解

如果您没有安装汉化补丁的话，本模组的设置文件（上文所述`config.json`文件)会在游戏带着此模组运行一次后自动生成。因此您也可以通过比对汉化补丁中提供的设置文件与自动生成的设置文件的方式自己动手汉化。

本仓库内提供的配置文件仅对需要中文化的字符串进行了改动，其他部分均为自动生成的设置文件的默认值。下面贴出了设置文件的内容全文，并在每一行之后进行注释，以对这些设置作简略说明。（注：添加注释是不规范的 json 用法，所以**不要**将这里的文本放到`config.json`内。）
```
{
  "modEnabled": true, //是否启用本模组，不要改动
  "isDebug": true, //是否以排错方式运行本模组，不要改动
  "RestrictBlocksToLandClaimArea": true, //是否将本模组的拾起物块功能限制在领地范围内
  "AllowToggleLandClaimRestriction": false, //是否运行在游戏内通过按键循环切换模组功能的启用范围
  "ToggleModKey": "p", //用于上述的循环切换的按键
  "EmptyFirstMessage": "拾起此容器前必须先将其清空", //翻译文本
  "DisabledText": "拾起物块功能已禁用", //翻译文本
  "RestrictionEnabledText": "拾起物块功能已限制在领地范围内启用", //翻译文本
  "RestrictionDisabledText": "拾起物块功能已无限制启用" //翻译文本
}
```
***
完
***