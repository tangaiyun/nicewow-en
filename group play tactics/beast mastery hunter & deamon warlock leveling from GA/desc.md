#### 简易宏设置样例
现有1猎人id为： 骑虎牵黄擎苍， 1术士id为：体柔身娇

猎人可以的宏的定义如下：

猎人1键位宏
```
#showtooltip 猎人印记
/petattack
/cast 猎人印记
```
猎人2键位宏 

```
#showtooltip 稳固射击
/petattack
/castsequence reset=12 毒蛇钉刺,稳固射击,稳固射击,稳固射击,稳固射击,稳固射击,稳固射击
/use 屠龙者的纹章
/use 沙虫之毒
```

猎人3键位宏

```
#showtooltip 奥术射击
/cast 奥术射击
/petattack
```

猎人4键位宏

```
#showtooltip 多重射击
/assist
/cast 多重射击
/petattack
```

术士1键位宏

```
#showtooltip 
/target 骑虎牵黄擎苍
/assist
/petattack
```

术士2键位宏

```
#showtooltip 痛苦诅咒
/target 骑虎牵黄擎苍
/assist
/petattack
/castsequence reset=12 痛苦诅咒,腐蚀术,献祭,烧尽,烧尽,烧尽,烧尽
/use 衰落之眼
```

术士3键位宏

```
#showtooltip 恐惧
/target 骑虎牵黄擎苍
/assist
/petattack
/cast 恐惧
```

术士4键位宏

```
#showtooltip 吸取灵魂
/target 骑虎牵黄擎苍
/assist
/petattack
/cast 吸取灵魂
```

术士T键位宏

```
/af 骑虎牵黄擎苍
```
术士G键位宏

```
/af stop
/f 体柔身娇
```

#### 典型打怪场景
- 玩家主控猎人，猎人选定目标按1键，则目标被标记，猎人的宠物会冲向目标并攻击，由于键位被复制，术士也会自动按1号键，术士的宠物也会冲向目标并攻击。
- 宠物开始攻击后，玩家不停按2号键，猎人和术士都会不停按照2号键位宏里定义castsequence 技能一次施放攻击目标
- 如果目标还没死亡，并向猎人靠近，玩家可以按3号键位，猎人施放奥术射击，术士施放恐惧，目标怪物会被恐惧逃跑
- 目标怪物在逃跑，血已经也不多了，玩家可按4号键，则猎人施放多重射击，术士施放吸取灵魂，准备收取灵魂石