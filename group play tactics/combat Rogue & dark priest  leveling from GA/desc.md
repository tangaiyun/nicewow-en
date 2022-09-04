#### 简易宏设置样例
现有1盗贼id为： macy， 1暗牧id为：milkcow

盗贼的宏的定义如下：

盗贼1键位宏
```
#showtooltip 影袭
/cast 影袭
/startattack
/equipslot 16 迈克斯纳之牙
/equipslot 17 末日先驱
/equipslot 10 古代熔火皮手套
/use 刃拳的宽容
```
盗贼2键位宏 

```
#showtooltip 刺骨
/cast 刺骨
```

盗贼F1键位宏

```
#showtooltip 剥皮
/equipslot 16 item:19901:803
/equipslot 17 item:19901:912
/equipslot 10 夜幕杀手手套
/cast 剥皮
```

盗贼键位布局图
![image](https://user-images.githubusercontent.com/7961235/188297647-2e59e405-236b-41cb-9dbd-13f9e8bc2410.png)


盗贼只有5个键位放置了宏, J键，Q键放置是空宏（里面没有任务内容的宏）

牧师1键位宏

```
#showtooltip 
#showtooltip 暗言术：痛
/target macy
/assist
/castsequence reset=12 暗言术：痛,心灵震爆,精神鞭笞
/use 伊利达雷的复仇
/use 闪耀水晶徽记
```

暗牧2键位宏

```
#showtooltip 精神鞭笞
/target macy
/assist
/castsequence reset=5 精神鞭笞

```

暗牧3键位宏，这是一个治疗盗贼宏

```
#showtooltip 恐惧
#showtooltip 真言术：盾
/target macy
/castsequence reset=12 真言术：盾,恢复

```

暗牧J键位宏，选贼盗贼目标快速治疗

```
#showtooltip 快速治疗
/target macy
/assist
/cast 快速治疗
```

暗牧Q键位宏，灭

```
#showtooltip 暗言术：灭
/target macy
/assist
/cast 暗言术：灭
```


暗牧T键位宏

```
/af macy
```
术士G键位宏

```
/af stop
/f player
```
![image](https://user-images.githubusercontent.com/7961235/188297666-85eb5176-b44d-49fc-b5a3-80974de96df6.png)



#### 典型打怪场景
- 按照盗贼的节奏打，先111，星快满了按2，如果盗贼血少了按3，连着按3会先给盗贼盾后恢复，如果怪血濒死了，按Q键呼叫暗牧的灭
