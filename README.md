# Nicewow

#### Introduce
A tool to WOW and SIMILAR ONLINE games more fun, especially for multi-boxing players

#### Installation

- Download the released version： [Release1.0.0 ](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-retail.zip)

- Decompress the zip file to any folder, and the folder content structure is as follows:
![image1](https://user-images.githubusercontent.com/7961235/188293687-ff516224-b5f9-4ff8-b3fb-23453f8bc614.png)



#### AutoFollow 插件安装
- 怀旧服安装AutoFollow插件到"World of Warcraft/\_classic\_/Interface/AddOns"目录
- 正式服安装AutoFollow插件到"World of Warcraft/\_retail\_/Interface/AddOns"目录
- 怀旧服插件版本下载地址 [怀旧服适用版本](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-classic.zip)
- 正式服插件版本下载地址 [正式服适用版本](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-retail.zip)

#### 软件运行                            
- 先多开运行游戏，本应用最多支持5开 
- 游戏已运行后，运行本软件。如果是怀旧服，运行wowclassic.bat, 正式服运行wow.bat

#### 启动后参数输入
启动后，程序需要你输入三个参数
- 请输入您的前进按键: 就是你魔兽里面人物前进的按键，大多数人应该都是W（不分大小写）
- 请输入召集跟随按键,注意这个键位将绑定跟随宏: 这个键位对于跟随者来说，绑定是跟随宏，默认值是T（不分大小写）
- 请输入停止跟随按键，注意这个键位将绑定停止跟随宏:这个键位对于跟随着来说，绑定是停止跟随宏，默认值是G（不分大小写）
- 跟随宏和停止跟随宏如何设定，[请参考核心宏设定小节](#核心宏设置)
- 一般的程序启动输入情况如图所示
![输入图片说明](%E5%90%AF%E5%8A%A8.jpg)

#### 功能初步验证
程序正常启动后，玩家操作主控角色，按一下空格键（Space），如果所有多开的角色都会同时起跳，说明键位同步功能已正常启用。

#### 核心宏定义及宏键位绑定

核心宏仅为二个, 因为玩家主要操作主控角色，那么所有跟随角色必须要做两个宏，即“跟随宏”和“停止跟随宏”

- 跟随宏 （建议放置在跟随角色的T键位上）
```
/af 主控角色id
```

- 停止跟随宏 （建议放在跟随角色的G键位上）
```
/af stop
/f player
```
#### 重要移动控制键位
- DEL键，键位同步开关键，用户可通过按DEL来关闭/打开键位同步功能，在非游戏的时候，关闭键位同步是个不错的主意
- 召集跟随键，默认是T，实际由用户启动时输入，命令所有跟随角色重新跟随主控角色的键位
- 停止跟随键位， 默认是G，实际由用户启动时输入，命令所有跟随角色停留在原地
- 主控前进键位，默认是W，实际由用户启动时输入，命令主控角色行走，插件也会根据此按键下按事件自动发送"召集跟随键"到所有跟随者客户端，命令所有跟随者重新跟随主控角色

#### 协同行动
- 玩家按一下T键，则跟随者会主动跟随主控角色。玩家按一下G键，则所有跟随者停留在原地。
- 经过测试，术士法师等职业施放瞬发和读条技能，不会脱离跟随状态，但是如果施放通道魔法（吸取灵魂，奥术飞弹等），则会脱离跟随状态。目前插件已经在绝大多数情况下，可以让跟随者自动重新跟随主控角色行动，如果在意外的情况下，跟随者没有及时跟上，可按一下T，主动让跟随者重新跟随主控角色。

#### 近战组合额外配置，近战跟随者需要额外配置如下
- ESC-界面-游戏-鼠标-点击移动（勾选）， 点击移动视角模式--总是调整视角
- ESC-按键设置-选中目标-与目标互动-K 
- 如果近战跟随者，离主控攻击的怪有距离，无法攻击到，玩家按一下K键，则近战跟随者会主动调整视角并靠近目标怪物攻击

#### 玩家已开发的玩法样例
- 每个玩家开发的样例占有一个目录，目录下至少有2个文件，一个是键位同步设置文件keyclone.txt,一个是md文件，描述了玩法角色的宏设定，键位宏绑定，以及一般的战斗过程描述。
- [兽王猎+恶魔术组合](https://gitee.com/aiyuntang/nicewow/tree/master/%E7%8E%A9%E6%B3%95%E7%9B%AE%E5%BD%95/%E7%8C%8E%E4%BA%BA+%E6%9C%AF%E5%A3%AB%20From%20GA)
- [战斗贼+暗牧组合](https://gitee.com/aiyuntang/nicewow/tree/master/%E7%8E%A9%E6%B3%95%E7%9B%AE%E5%BD%95/%E7%9B%97%E8%B4%BC+%E6%9A%97%E7%89%A7%20From%20GA)

#### 视频攻略
- [自动跟随重生，nicewow让你多开体验重回巅峰](http://https://www.bilibili.com/video/BV1Pd4y1V7Aw)
- [WLK如何愉快的玩耍,多开党的福利送到](https://www.bilibili.com/video/BV1de4y1a7iU/)

- [正式服支持以及近战组合练级心得](https://www.bilibili.com/video/BV13P411V7eu/)


#### 软件密钥设置
- 软件密钥定义在key.txt内，用户只有得到合法的密钥后并复制到key.txt内，本软件才能正常使用

- key.txt初始内容为试用key，可能会过期

- 从管理员得到key后，运行该软件后，key会跟当前电脑绑定

#### 键位同步设置 keyclone.txt

- 本软件内置可同步的键位为：` **A-Z(26个字母键),  0-9（10个数字键）， SPACE(空格键），OEMMINUS（减号），OEMPLUS（加号）, F1-F12(12个功能键）** `

- 用户可自定义被同步的键位，打开keyclone.txt, 初始内容为： 

```
D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 SPACE W E J Q T G Z X Y K H OEMMINUS OEMPLUS F1 F2
```

  初始键位同步设定含义为： 数字键0-9，空格键，字母键 W E J Q T G Z X Y K H, 减号, 加号,F1,F2 这些键位会复制，其他键位会忽略 

- 用户可自行增加或者减少里面定义的键位，但是增加的键位仅允许在本软件内置可同步的键位内。

- 本软件仅会同步在keyclone.txt里定义的键位，其他未出现在keyclone.txt里的键位会被忽略


#### 其他MMORPG网游支持（实验性，有效性有待玩家探索）
- 多开网游客户端
- 按CRL+ALT+DEL键，打开windows 任务管理器，选则详细信息Tab页，找到该网游客户端的进程，例如魔兽怀旧服的进程如图所示
![输入图片说明](taskmanager.jpg)
- 假设该网游的客户端的进程名称为 xyz.exe
- 在软件目录下制作一个文本文件，xyz.txt,里面的内容如下

```
@echo off
start NiceWow.exe xyz
exit
```
- 改变xyz.txt后缀名为bat，则软件文件目录结构类似
![输入图片说明](xyz.jpg)
- 多开玩游xyz，点击运行xyz.bat即可


#### 技术支持
- 微信： zhuiyingderen
- QQ： 15520929

#### 开源合作
- 欢迎各位爱好者提供玩法PR
- 玩法PR请在目录 "玩法目录"里建立你自己的目录
- 你自己的目录下至少包含2个文件，1个为keyclone.txt，描述了你要键位复制的配置，另外一个为md文件，描述键位上宏的设定，以及典型玩法描述
- 如果你有更好的想法，请你体现在你的PR里，欢迎之至
- 玩法PR review通过被收录，免费送月卡1张

#### 软件试用和收费

- 下载后可免费试用一周
- 长期使用月卡19.9元一张，支持5号同开，良心价格，童叟无欺
- 朋友圈转发消息截图，再送1周 
- 推荐一人购买一张月卡以上，送月卡一张


#### 免责申明

- 本软件完全出于个人兴趣爱好，由本人在业余时间开发，是一款安全，绿色，可靠的软件产品
- 本软件不会收集任何用户数据，使用时无任何网络通讯,欢迎任何专业人士验证
- 利用本软件所做出的任何行为，和本人无关
- 因使用本软件而引致的任何意外、疏忽、合约毁坏、诽谤、版权或知识产权侵犯及其所造成的任何损失，本人概不负责，亦概不承担任何民事或刑事法律责任
- 当你第一次开始使用本人所提供的任何软件及资源的那一刻起就将被视为对本声明全部内容的认可。同时您必须认可上述免责条款，方可使用本软件及资源。如有任何异议，建议立刻删除本软件及资源并且停止使用
- 以上内容，本人保留最终解释权
