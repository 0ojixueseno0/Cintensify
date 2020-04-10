
![](https://gitee.com/im0o/photobed/raw/master/img/20200410213319.png)

# Cintensify

功能简单指令简单配置简单的极简的自定义强化物品插件

## 插件功能
输入指令，消耗点券，强化手中物品（添加lore）
## 指令＆权限
\[Cintensify] 强化 帮助
```
- cintensify.use
/ciy help - 查看帮助
/ciy i - 消耗20点券强化手中的物品
- cintensify.admin
/ciy reload -重载插件
```
## 配置文件
```
#C_intensify 自定义强化配置文件

#插件版本，请勿更改
version: 1.0
#强化失败后的信息
failmsg: "§a[Citensify] §c强化失败"
#强化等级
levels:
#等级(等级之间之间必须按照顺序排序，不可出现跨度/乱序)
  1:
#成功几率(x分之1 数字越大几率越小 数字不能小于1)
    chance: 1
#增加的lore(每次强化都会给物品新增一条lore)
    addlore:
    - "§f--------强化栏--------"
    - "§a攻击力: +10"
#强化成功后的信息 %player%=玩家名 %name%=装备名 %level%=强化等级
    playermsg: "你成功将装备强化到了1级"
#强化成功后是否开启公告
    enablebc: true
#公告内容(enablebc=true后必填)
    bcmsg: "%player%成功将装备%name%强化到了%level%级"
  2:
    chance: 10
    addlore:
    - "§a攻击力: +10"
#playermsg为none即为不提示玩家
    playermsg: none
    enablebc: false
```
## 前置插件
PlayerPoints(MCBBS)：[点击访问](https://www.mcbbs.net/thread-461244-1-1.html)

Skript(github)：[点击访问](https://github.com/SkriptLang/Skript/releases/tag/2.3.7)

skyaml(github)：[点击访问](https://github.com/Sashie/skript-yaml/releases/tag/v1.3.2)

TabooSK(MCBBS)：[点击访问](https://www.mcbbs.net/thread-692070-1-1.html)
