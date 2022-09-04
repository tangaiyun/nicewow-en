# Nicewow

#### Introduce
A tool to WOW and SIMILAR ONLINE games more fun, especially for multi-boxing players

#### Installation

- Download the released version： [Release1.0.0 ](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-retail.zip)

- Decompress the zip file to any folder, and the folder content structure is as follows:
![image1](https://user-images.githubusercontent.com/7961235/188293687-ff516224-b5f9-4ff8-b3fb-23453f8bc614.png)



#### AutoFollow addon installation
- WOW classic put AutoFollow to the folder "World of Warcraft/\_classic\_/Interface/AddOns"
- WOW retail put AutoFollow to the folder "World of Warcraft/\_retail\_/Interface/AddOns"
- [classic version](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-classic.zip)
- [retail version](https://github.com/tangaiyun/nicewow-en/blob/main/AutoFollow-retail.zip)

#### start                            
- for classic wow，please run wowclassic.bat
- for retail wow, please run wow.bat

#### Parameters
Once started, the program requires you to enter three parameters
- Please input you key for moving forward, the default value is W: W
- Please input your key for following, the default value is T: T
- Please input your key for stopping following, the default value is G: G
- Program startup input is shown as Figure
![image](https://user-images.githubusercontent.com/7961235/188293912-0b2b2359-58ce-4602-9a83-4d46a07ccd43.png)


#### Preliminary functional verification
After the program starts normally, the player can operate with the leader role wow window and press the Space bar. If all the wow characters jump at the same time, it means that the key synchronization function has been enabled normally.

#### Core macro definitions and key bingding

There are only two core macros, because the player mainly controls the leader character, so all the following characters must make two macros, namely "Follow macro" and "stop following macro".

- Follow Macro （bind to Key 'T）
```
/af leader's id
```

- Stop Following Macro （bind to key 'G'）
```
/af stop
/f player
```
#### Important movement control key
- 'DEL': turn on/off key synchronization by pressing DEL. It is a good idea to turn off key synchronization when you are not playing games
- 'T' : press this key to let all follower characters to follow the leader character
- 'G' : press this key let all all follower characters to stay where they are 
- 'W' : player press this key to let the leader character to move forward, at the same time, this tool will send 'T' key press event to all followers automatically, then followers will follow the leader again 

#### Team movement
- When the player presses the T button, all followers will follow the leader character. The player presses the G button, and all followers where they are
- some classes such as mage or warlock, when they cast channel spells, then their following state will be lost, but this tool has enabled the followers to automatically follow the leader again in most cases. If the follower fails to follow the leader role in time under unexpected circumstances, you can press T 
to let the followers follow the leader again.

#### Additional config for melee follower
- ESC- Interface - Games - Mouse - Click Move (checked), click Move View Mode - always adjust the view
- ESC- Key Settings - Select Target - Interact with target -K
- If the melee follower is far away from the monster which leader is attacking, the player should presses the K key, then the melee follower will actively adjust its perspective and move close  and attack the monster

#### Some group play tactics 
- each group play tactics has one dirctory. under the directory, There are at least 2 files in the directory, one is keyclone.txt file, and one is MD file, which describes the macro Settings, the key macro binding, and the general battle process description.
- [beast mastery hunter & deamon warlock](https://github.com/tangaiyun/nicewow-en/tree/main/group%20play%20tactics/beast%20mastery%20hunter%20%26%20deamon%20warlock%20leveling%20from%20GA)
- [combat Rogue & dark priest](https://github.com/tangaiyun/nicewow-en/tree/main/group%20play%20tactics/combat%20Rogue%20%26%20dark%20priest%20%20leveling%20from%20GA)

#### Key Setting
- the key is defined in key.txt. The tool can be used normally only after the user gets the valid key and copies it to the key.txt
- the original key.txt contains a trial key and it may expire
- After getting the key from the admin and running the tool, the key will be bound to the current computer
- 
#### Key Multicasting Config --- keyclone.txt

- The built-in sync supported keys of this tool is：` **A-Z,  0-9， SPACE，OEMMINUS，OEMPLUS, F1-F12** `

- You can customize your keys to be synced by modifying the file keyclone.txt
- Open the keyclone.txt, the original content should be ： 

```
D0 D1 D2 D3 D4 D5 D6 D7 D8 D9 SPACE W R U I E J Q T G Z X Y K H OEMMINUS OEMPLUS F1 F2 F3 F4
```

  it means： gigit keys 0-9, space bar, letter keys W R U I E J Q T G Z X Y K H, minus sign, plus sign,F1,F2,F3,F4 These keys would be synced, other keys will be ignored

- Users can add or reduce the keys defined in keyclone.txt, but the added keys are only allowed in the software built-in synchronized keys.


#### other MMORPG game support（Experimental, effectiveness should be explored by players）
- press CRL+ALT+DEL，open windows task manager，select detail Tab, to find the game process name, for wow classic, the name is WowClassic.exe
- Assume that the process name of the online game is xyz.exe
- Make a text file named as xyz.txt, which contains the following contents

```
@echo off
start NiceWow.exe xyz
exit
```
- If you change the file name of xyz.txt to xyz.bat
- run xyz.bat


#### Technical support
- Mail: aiyun.tang@gmail.com
- Wechat： zhuiyingderen

#### Open source cooperation
- Welcome fans to provide group play PR
- if you want to make a pull request, please create your directory under the folder 'group play tactics'
- your own directory should contain at least two files: keyclon.txt, which describes waht keys you wants to sync, and desc.md, which describes the macro definition and key binding, talent etc.
- ff you have a better idea, please represent it in your PR

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
