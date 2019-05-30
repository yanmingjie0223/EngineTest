EngineTest
* 下面是针对CocosCreator2.0.6和laya2.0 beta5版本对比，对比方式是相同的数量的骨骼动画和帧动画，比较占用内存/cpu及渲染统计。
* 这里会使用到nginx，游戏访问/包括后面微信打包res资源目录的转移

内存与cpu占用（帧动画和骨骼动画）
* ![cocos_骨骼_内存](/Image/cocos_骨骼_内存.png)
* ![laya_骨骼_内存](/Image/laya_骨骼_内存.png)
* ![cocos_帧_内存](/Image/cocos_帧_内存.png)
* ![laya_帧_内存](/Image/laya_帧_内存.png)
* 根据得出的结果无论是帧动画还是骨骼动画laya都跟为良好，骨骼动画差距比较大
* cpu是浮动的，帧动画中浮动非常的接近laya还是占用少一点，骨骼动画差距比较明显

微信上帧数、发烫（测试手机iPhone 6 10.3.3）
* ![微信统计](/Image/微信上统计表.png)
* cocos creator发烫更为明显，这里就没有做温度统计

注：这里的骨骼动画都是龙骨动画，目前龙骨使用还是比较多的（后面coco creator优化，内存占用差距是比较接近，太懒没有整理相关数据）
