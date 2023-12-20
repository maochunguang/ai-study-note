# 本地运行大模型准备

## 硬件准备
### 1、硬件准备
1、物理机：内存建议32g或者以上，gpu显存建议至少16g，特别是如果跑图片的话，20g会更好。显卡我推荐一个性价比比较高的魔改版2080ti,2700左右的价格，22g显存，性价比算是很高了。如果不是编程编程专业不建议用amd显卡，真的是浪费时间。如果是高端又追求性价比的可以买2个或者4个2080ti，性价比也非常高，显存会非常足。

2、云主机，不想买物理主机的，建议使用阿里云或者其他厂商的gpu机器，按流量或者时间计费，尝尝鲜也是很不错，比买显卡便宜多了。

### 2、系统和环境准备

#### 第一种系统：win11+wsl2
适合window生态的玩家，不用切换系统，平常想打打游戏啥的不耽误，想跑跑模型，打开wsl2开箱即用。
* 优点：不用切系统，可以打游戏，非常方便
* 缺点：跑gpu的性能比linux会低一些，个人感觉完全够用。

#### 第二种系统：ubutun22.04系统，
适合高级选手，以及生产力玩家。装ubutun后基本上告别了游戏，除非你装个双系统。

#### 其他环境
##### 1、安装python
