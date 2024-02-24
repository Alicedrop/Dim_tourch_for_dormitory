# 适合宿舍的微光手电筒 Dim_tourch_for_dormitory
为晚上在宿舍学习不打扰别人设计的手电筒。

A tourch designed to study in the dormitory at night without disturbing others.

这是为了晚上在宿舍学习、看小说不打扰别人，也不容易被宿管发现而设计的手电筒（我们高中抓手电筒）。它的亮度合适，可以在床上看书，可以根据需要用电位器调节到合适的亮度。
特别适合晚上在宿舍床上学习不影响到别的同学，又能保证较为充足的光线照亮书本
尽管这玩意儿几乎没有技术含量，但是真的好用。

使用CR1220纽扣电池供电，电位器调到平时阅读的亮度一直开着，可以连续发光1个月以上，正常使用的话续航很长。

项目使用立创EDA绘制，提供的是立创EDA的工程文件，也可以在[release](https://github.com/Alicedrop/Dim_tourch_for_dormitory/releases)处下载gerber文件直接去打板。
立创开源广场的链接：
https://oshwhub.com/18102521490aa/mi-l_copy

![image](https://github.com/Alicedrop/Dim_tourch_for_dormitory/assets/128953967/1079138d-0497-4727-b945-bcccdd446c3c)

![image](https://github.com/Alicedrop/Dim_tourch_for_dormitory/assets/128953967/d134ebe8-1270-4ea2-9bdd-ba882e41fc01)

## M.L系列和Slice系列
这个项目我从初三开始做，一共迭代了10次，最开始是M.L系列，M.L v6之后为了轻薄化转为开发Slice系列。最后一次修改是大一。
![image](https://github.com/Alicedrop/Dim_tourch_for_dormitory/assets/128953967/d60a3e8e-cdba-40ba-846f-228d89e55968)
![image](https://github.com/Alicedrop/Dim_tourch_for_dormitory/assets/128953967/f6778abc-02ba-4dd4-bc99-0d9b0e08a147)

Slice加入了一定的人体工学设计，并且故障率降低了很多，如果想做的话建议做Slice系列。

## 制造工艺注意事项
1. R1使用的“旋转电位器YEP”封装是我画的，购买时搜索拨盘电位器即可。
2. 注意，发光二极管要买圆头的（顶部是个半球，形成凸透镜），这样才能汇聚光线，实现很小的功率便能照亮书本，同时其他方向光较少亮度衰减很快，在能看书的同时不容易影响别人、被宿管发现。
3. 如果像演示图那样，把LED弯折90°焊接上去，需要在PCB两面都进行焊接，否则由于挤压磕碰会导致LED松动，灯光出现闪烁。
4. 建议完成后把电池用绝缘胶布包着，底面也贴上绝缘胶布，用热风枪或电吹风加热至软化，冷却后胶布会表现出类似热缩管的特性，变硬且不容易脱落。这样可以保护电池、防止引脚刮坏物品以及减少使用者与焊点的接触。

## 故障排除
以下是在长期的开发和使用中总结出的故障排除。
1. 如果灯光出现闪烁，首先检查LED是否松动，以及是否抓握时手指挤压电池、电位器。如果都不是，再考虑其他问题。
