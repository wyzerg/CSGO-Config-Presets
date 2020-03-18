# [CS:GO] Cfg-Preset-By-Purp1e
>这是我个人写的CSGO config的预设，包含各种应用场景，注释详细

>涉及很多日常使用的指令和功能（服务器指令pass），实时修改更新

>对接触csgo指令不熟悉的人和想方便改变、转移设置等玩家都有很大帮助

## Cfg Preset v1.3d

1. 修复**stream.cfg**的错误

## Cfg Preset v1.3c

1. 修复**practice.cfg**中的速度不正常的问题
2. 跑图**practice.cfg**中添加一键加速时间的功能，默认键位`。`，松开恢复，但是帧数会骤降，队友会卡住，可以适当降低数字`25`到`20`~`25`
3. 可选指令中增加`virre`的白色准星参数
4. **hlae.cfg**中增加去除所有天空的云朵的快捷键`\`，切换天空skybox的控制台提示改为中文，镜头录制模式默认使用第三人称自由视角
5. 一键高亮和隐藏HUD的快捷键互换，高亮为`J`，后者为`H`，一键高亮逻辑重写，现为V4版本，新增指令`assist` `onred` `offred` `skip` `debug`
6. ffmpeg录制预设参数优化，加入prores编码的预设，减少最多50%文件体积
7. **stream.cfg**逻辑重写，F1~F9切换某个通道的不同类型 统一由Insert键开启，Delete键关闭，F11关闭预览、打印所有通道信息，F12删除所有通道、重置状态
8. 修复**export.cfg**打印的参数顺序
9. **auto.cfg**中增加加载hlae.cfg的快捷键，默认关闭
10. 新增`DLC_v1.3c.zip`用于AE中制作HUD

## Cfg Preset v1.3b

1. 修复了1.3a使用说明中二维码不显示的问题（恰饭大失败）
2. "可选指令"中加入了单独的自动投掷物准星，仅可搭配基础跳投使用；加入了按键式开关投掷物准星的代码，一开一关；加入了一开一关的开放式麦克风的代码（慎用）
3. stream.cfg指令优化，现在切换不同通道的预览时会重置其他通道的指令状态，使用更加方便
4. 修复了hlae.cfg中录制帧率快捷指令的一些错误，修改了切换自带天空贴图指令的按键以兼容stream.cfg，现为`q`；增加了导入导出镜头路径的提示指令`hint`
5. 极大地改进自拍杆cals.cfg，现在按键`[`切换锁定的玩家，按`]`切换6种自带预设视角，`cls`指令还原正常视角，`exec cals`重新加载自拍杆，现在不用手动打开cfg修改代码了

## Cfg Preset v1.3a

1. 修复了hlae.cfg的一处提示错误，修复了一键高亮的小问题，添加了@dq-CSGO提供的切换多种天空贴图skybox的指令，默认为按键`P`
2. 修复了cals.cfg的编码问题，现已经转换为utf-8，不会出现乱码了

## Cfg Preset v1.3

1. auto.cfg
   - 默认关闭鼠标加速
   - 优化预设屏幕亮度 现为1.8 偏亮
   - 添加固定滚轮跳的指令 原先鼠标中键切换滚轮跳和切枪的指令、以及左上角显示伤害的指令移动到了`可选指令`中

2. demo.cfg
   - 添加了指令mute，可将MVP、回合开始、结束等声音关闭
   - 移除了有BUG的更改FOV的指令

3. practice.cfg (配合knife.cfg)

   - 添加了本地bhop的指令，快捷键`P`
   - 添加了本地分批次生成各种原版刀的指令和键位，必须有knife.cfg在同目录才能生效，玩家须装备原版刀否则只会掉落当前的刀，快捷键`9`, `0`, `-`, `=`

4. hlae.cfg

   - 移除了有BUG的更改FOV的指令，添加了新的更改FOV指令，键位`-`, `=` 分别对应FOV=105和默认值，同时加入修复开镜BUG的指令
   - 改进了一键高亮击杀信息的指令，现在为4个状态：红框-关-透明框-关，避免了一些蜜汁BUG，**键位更改为`H`**
   - 添加了屏蔽某个、一边（T/CT）玩家语音的指令提示
   - 添加了修改玩家名称的指令提示
   - 添加了指令mute，可将MVP、回合开始、结束等声音关闭
   - 修改了默认开启raw通道的指令，现在固定开启raw通道，分层录制的更详细更方便的指令单独出来成为stream.cfg
   - 提供一些可能有用的预设并注释

5. stream.cfg（终结HLAE分层录制问题）
   - 新添加的CFG，内置十种总结好的通道设置，使用F区的按键
   - F1~F10分别对应其通道，每个按键按第一次开启并设置好该通道，按第二次开启该通道的录制，按第三次关闭该通道的录制
   - F11关闭通道预览并打印通道信息，F12删除所有通道并还原F1~F10的指令状态
   - 配有全中文控制台提示

6. cals.cfg
   - 自拍杆CFG，里面包含先前dq总结过的指令
   - 添加了`clearcals`指令，使用该指令可以清除自拍杆设置，再次加载CFG再次开启自拍杆
   - 添加了若干自拍的预设指令，配有全中文控制台提示
7. 使用说明
   - 细节优化
   - 添加了支付宝二维码，可以通过捐助的方式支持我的工作
8. 武器购买代码表
   - 补上了缺少的匪喷的代码
9. 可选指令
   - 如1中所说
   - 感谢贴吧 @风起天澜555 提供的一些指令，请根据需要自取
   - 添加固定的WASD修改HUD颜色的指令，不像之前那么杀马特了

## Cfg Preset v1.2d

1. 文本文档全部改用Markdown格式书写并导出的HTML页面

## Cfg Preset v1.2c

1.核心auto.cfg中加入voice_enable指令，以防使用demo/hlae.cfg后游戏队内交流语音被关闭

2.更新显示队友位置和装备的指令cl_teamid_overhead_mode，原指令已失效

3.添加cl_crosshair_friendly_warning指令[auto.cfg 73行]，设置成2后瞄准队友时会叠加一个褐色的默认静态准星

4.“可选指令.txt”中加入了杀马特的鼠标左键切换准星颜色和WASD切换UI颜色

## Cfg Preset v1.2b

根据9.20的更新进行若干修改

1.跑图用practice.cfg中添加T键重现最近一次的投掷物（同nadetraining插件）

- 增加实时预测轨迹的指令键位"，" 和预测投掷物轨迹的按键'[' ']' 分别为30/100s（按一次触发一次）
  
- 增加修改半甲/全甲的指令提示等
  

2.修复hlae.cfg中一键高亮的键位提示错误  应为q键  增加若干提示

3.使用说明中增加对各个文件作用的描述

4.添加了2个无聊的小彩蛋

## Cfg Preset v1.2a

适配HLAE新版本特性(1和2必须使用hlae开启CSGO才有效)

1.增加上一回合/下一回合的指令及快捷键"," "."  修改一键高亮击杀快捷键为"q"

2.一键高亮击杀等功能现在在控制台中显示中文提示

3.增加判断是否成功使用hlae打开csgo的指令，成功时显示

```
HLAE启动状态

成功√
```
失败时显示
```
HLAE启动状态：

x
```
## Cfg Preset v1.2

1.新增export.cfg，使用预设之前单独加载该cfg可以显示准星+持枪参数

2.跳投全部调整为双键，现在右键也可以使用跳投

3.丰富了启动项说明

4.新增ffmpeg.cfg和ffmpeg420.cfg，用于搭配hlae录制集锦素材

5.hlae.cfg新增天空贴图skybox相关指令快捷键，预置几个天空贴图指令

6.修复若干说明错误，细节进一步优化

## Cfg Preset v1.1

1.auto.cfg中恢复基础跳投、基础投掷物准星

   【防误触跳投+自动投掷物准星+个性化左右手】相关指令移到"可选指令.txt"

   因为这些功能之间有交集 所以针对不同的情况分别给出了代码

   现在直接复制对应代码 覆盖auto.cfg中对应位置即可

   请根据个人需要自取

2.demo.cfg中现在按p切换demo暂停/继续，取消之前的'['和']'键

3.删除了demo.cfg中和hlae相关的指令

   新增hlae.cfg 包含很多demo、hlae相关指令(一键高亮等)

4.solo.cfg增加solo模式的选择

   控制台输入如aksolo或者按下设定好的按键(7890-=)

   可以设置好出生武器并重新开始游戏

5.solo.cfg中默认100回合

6.新增"可选指令.txt" "使用说明.txt""武器购买代码.txt"

7.其它细节优化

### 使用视频：

#1 AV34054584 前7分钟

#2 AV34789804 (终结篇)

#3 AV45088666 (转移设置脚本)

#4 AV47120170 (v1.0使用说明)

#5 av51220317 (v1.1使用说明)

#### Cfg Preset By Purp1e

链接:https://pan.baidu.com/s/1m91kr2eqH68sYSZgsPP38A

提取码:vh21

### 各文件功能预览

#### 1.auto.cfg

目录  亮度设置  准星设置 鼠标设置

基础设置  持枪视角设置 HUD设置

音量设置  绑定清血迹  解绑按键避免冲突

滚轮跳+中键切换(声音提示)

大跳 基础跳投+投掷物准星

切换左右手  单独绑定投掷物

快速购买武器

使用提示

#### 2.crosshair.cfg

准星修改提示

准星参数

#### 3.crosshair_throw.cfg

投掷物准星参数

#### 4.practice.cfg

开启作弊 各项参数修改

投掷物、弹着点轨迹

金钱、时间修改

全图、任意时间购买

全枪全弹（掉一地枪）

绑定按键（bot操作）(开关轨迹、透视模式等)

使用提示

#### 5.solo.cfg

开启作弊 各项参数修改

可选solo模式 按7890-=键分别切换不同模式

回合开始1s等待

回合结束2s等待

金钱、时间修改等

使用提示

#### 6.demo.cfg

绿色静态准星 集锦专用持枪

暂停demo

绑定按键（暂停继续雷达等）

鼠标前后侧键切换demo播放速度

还原默认HUD设置

使用提示

#### 6.hlae.cfg

hlae相关参数设置

绿色静态准星 集锦专用持枪  还原默认HUD设置

暂停demo   绑定按键（暂停继续雷达等）

鼠标前后侧键切换demo播放速度

一键高亮击杀V2

使用提示

#### 6.export.cfg

显示准星+持枪视角参数

【防误触跳投+自动投掷物准星+个性左右手+快速切换道具】

6种不同需求组合的代码

#### 6.可选指令.txt

网络参数可选指令 双键跳投

【防误触跳投+自动投掷物准星+个性左右手+快速切换道具】

6种不同需求组合的代码
