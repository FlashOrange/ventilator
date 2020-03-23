Last updated 2020/03/20

![Full System](https://github.com/jcl5m1/ventilator/blob/master/images/full%20system.jpg?raw=true)

# 低成本开源呼吸机

NOTE: 本项目克隆自独立开源项目，特别需要注意的是，按本项目制造的器械，并不符合中国或其他国家对于医疗器械的要求，仅可以在非常规限定条件下使用，使用时需要在有执业资格的专业医师指导下进行。本项目仅为记录文献，并不为此项目所涉及的硬件中的部分或整体导致的任何事故负责。在没有正确指导的情况下使用未经过认证的医疗器械，可能会导致死亡！

* 2020年，COVID-19 病毒席卷全球，并且耗尽了多个国家的医疗资源.  本项目记录了将一种CPAP(持续气道正压) 充气机改造成一个压力支持无创通气机的过程，希望能够帮助在呼吸窘迫发生时得不到医疗支持的人们. 这是一个目前持续更新的项目，到目前为止，本项目涉及的设备，比较符合对于无创压力支持BiPAP呼吸机的定义。
 * 本项目同时也可以用于制造动力呼吸面罩 [低成本动力空气净化呼吸器 (PAPR)](https://github.com/jcl5m1/ventilator/wiki/Build-a-Low-Cost-PAPR) .  PAPRs 是个人防护装备的有效组成部分 (PPE)，用以帮助护理人员. PAPR在目前的情况下也非常紧缺，DIY此设备所带来的风险要远远低于DIY前面所述的呼吸机. DIY个人防护装备，给予陪护人员帮助，相对DIY呼吸机更加能够挽救人们的生命.  除非你有足够的专业能力参与到本项目相关的呼吸专科的专业讨论中，而又想提供帮助，建议从这里开始，而不要去DIY呼吸机.


### 警告与声明: 如有可能，请寻求专业的医疗护理，并由受过培训的个人设置适当的设备。不要随意使用你在互联网上找到的信息。我不是医学专业人士，只是一个把信息放到网上的人。在没有医疗监督的情况下，使用高压BiPAP来DIY呼吸机存在非常非常大的风险。  

### DIY呼吸机的主要风险
 * 只有在没有其他任何办法的时候，在一切资源都无法得到支持的时候，才可以去尝试用这里的方法DIY呼吸机，并且务必要在专业人员在场的情况下使用。这里为绝望的人们提供最后的希望（并且希望人们永远不要用到它）。
 * 无创呼吸机的使用可能会导致大量气溶胶的产生，这对周围的人们是非常危险的.  使用的环境应当在已经不能再糟糕的环境（气溶胶已经充满空间）. <strong>NOTE: 在共享通风管道和下水道的公寓中自我隔离，并不是一种合理的方案（这也是建立方舱医院的原因）.</strong>
* 在缺乏肺顺应性的条件下过高的压力(例如20cmh2o 或更高) 会损伤发炎的肺组织.  而目前的设计中并不包含相应的功能.
* 查看这里 [关于风险和工程控制的讨论](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist).

### 风险太高了? 做一个低成本PAPR吧!
再说一遍, 一个 [低成本主动空气净化呼吸器(PAPR)](https://github.com/jcl5m1/ventilator/wiki/Build-a-Low-Cost-PAPR) 能够给陪护人员提供很大的帮助，比被动式呼吸器要有效得多。

### 硬件要求和关于医疗器械的政府相关法规:
 * [中国关于医疗器械的相关法规](http://www.nmpa.gov.cn/WS04/CL2178/)
 * Requirements doc from [Code Life Ventilator Challenge - Montreal General Hospital Foundation](https://www.agorize.com/en/challenges/code-life-challenge/pages/guidelines?lang=en) (加拿大)

 * Requirements from [Gov.UK  - Rapidly Manufactured Ventilator System](https://www.gov.uk/government/publications/coronavirus-covid-19-ventilator-supply-specification/rapidly-manufactured-ventilator-system-specification?fbclid=IwAR2IgOyENgHJTsLouIiikpuiwgwupdB8d8Aun2he8nzMPWGfhBVhaG_sMqo) (UK)

### 当前的硬件功能
  * 这种初步设计可以有一个可编程的呼吸频率 (ex: 10-16/min)
  * 它可以设定呼气末正压(PEEP)
  * 呼吸机的气道压力可以高达 45cmh2o. 但是, <strong>[高于 20cmh2o 就会有危险](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist)</strong>.  
  * 它还无法设定适当的潮汐量，100毫升还是10毫升，多少是正确的？并不清楚。  
  * 它并不能调节氧摄取分数(FiO2).  但是，连接到氧气罐的下游可以通过手动调节流量来提高氧气罐的浓度。我可以用一个指针指向一个低成本的O2传感器。
  * 这个项目的功能还很不完善，但当不能得到更好的治疗时，这种有限的功能可能会有所帮助。这也是取得进展的起点。关键功能可以随着时间的推移而增加。

这个发布于2020年3月17日的油管视频，演示的相关的部件:
[![Youtube video](https://img.youtube.com/vi/n57u1NvXBgw/0.jpg)](https://www.youtube.com/watch?v=n57u1NvXBgw)

还有一些其他的工作.  [一个简要的列表](https://github.com/jcl5m1/ventilator/blob/master/resources.md) Thanks! [discussion](https://github.com/jcl5m1/ventilator/pull/20) 



# To Do列表(一些事情我需要亲们的帮助):
 * 我和一位呼吸科科医生进行了长时间的交谈，讨论了合适的呼吸机的关键特征和权衡。 [这里是过程记录](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist).  如果你认识相关的专家，请帮助确认这部分讨论的合理性，这对今后的工作至关重要。
 * 开发一个简单的传感器 [通过呼吸机循环显示提供一个类似的肺顺应性近似值](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist#at-a-high-level-the-goal-is-to-get-enough-air-into-the-lungs-to-keep-the-patient-alive-without-causing-unnecessary-stress-on-infected-lung-tissue)
 * 一个 [内联空气过滤器的3D模型](https://www.directhomemedical.com/cart/merchant.mvc?Screen=PROD&Product_Code=1-H1605-inline-bacterial-viral-cpap-filters&Store_Code=DHM&gclid=EAIaIQobChMIo-G35omi6AIVSrzACh29hwv3EAQYASABEgK9FPD_BwE) 用来放置通用过滤片 [例如这样的](https://www.amazon.com/3M-Particulate-Filter-Organic-Filters/dp/B079X5C3QP/ref=sr_1_2?keywords=p100+air+filter&qid=1584469511&sr=8-2).
 * 肺模拟器的采购与支持. 这有一个高端的（太贵了） [Michigan Instruments](https://www.michiganinstruments.com/lung-simulators/adult-test-lung-simulators/).
 * 流量阈值告警.
* 一个能帮助我们找到好的零部件供应商的供应链人员，如果有意愿的话。我没有建立供应链。我手头上的少数几个零件可能没有持续性。
 * 弄清楚如何重新编写现有的BiPAP。如果这种操作模式有帮助，那么在这个领域中已经有大量这样的设备可以启用。我没有关于不同品牌/型号受欢迎程度的统计数据。 在没有疫情的情况下，全球也有[100万的此类设备需求](https://www.cheapcpapsupplies.com/blog/sleep-apnea-statistics/) ?
 * 修改设计，使其能够收集废气，以减少添加病毒传播。这只适用于已经“肮脏”的环境，那里很可能已经有含有病毒的飞沫在空气中传播——比如被隔离的空间或其他负压环境。
 * 开发Arduino兼容算法，通过[查看风机的背压负载](https://github.com/jcl5m1/ventilator/wiki/Breathing-Back-Pressure-Data-Analysis)将风机周期与呼吸周期对齐, 或非常简单的空气压力传感器，可以插入到泵的输出中.  为了便于开发算法，请参阅[带有数据可视化的 Colab notebook.](https://colab.research.google.com/drive/1iFMmMMrg_3OeifzJikT75fy4ev84W235)
 * 断电时的解决方案，我不知道怎么做，欢迎提供方案。
 * 测试一个[简易的充气泵](https://www.amazon.com/gp/product/B013UQ0T2Y/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) 并实现压力控制.
 * 开发一个低成本的流量传感器/逼近器 [用于控制流量](https://www.acepnow.com/article/avoid-airway-catastrophes-extremes-minute-ventilation/). 重症监护的流量达到 10-12L/Min.

可以通过[开一个新的 issue](https://github.com/jcl5m1/ventilator/issues) 来提供帮助，谢谢!


# 关于供应短缺的有用的参考资料/文档，以及关于未经批准的设备的指导:

关于未经批准的设备使用指南的有用文件越来越多，有关通风设备和个人防护设备估计短缺的信息也越来越多.  我们将这些信息转移到了这里 [Wiki可以更好的跟踪更新](https://github.com/jcl5m1/ventilator/wiki/Useful-References) 使其易于维护.

# Materials
1. [持续正压 (CPAP)](https://en.wikipedia.org/wiki/Continuous_positive_airway_pressure) 设备通常用于个人应对 [睡眠障碍](https://en.wikipedia.org/wiki/Sleep_apnea). 因此，CPAP鼓风机部件相当丰富. 可以在ebay上获得二手的，在阿里巴巴上可以找到新的（译者注：阿里国内1688网站上有，淘宝上没找到）. 在这些设备中，鼓风机是一个简单的无刷直流电动机，它可以由一个电子速度控制器(ESC)驱动，该控制器可以用于无人机和遥控车.  The 我从这里拆了一个 [Respironics REMStar](https://www.google.com/search?q=respironics+remstar&safe=off&rlz=1C1CHBF_enUS809US809&sxsrf=ALeKk00Uw98vXCAyCiiSglgt-2Ucnz5RCg:1584357572342&source=lnms&tbm=isch&sa=X&ved=2ahUKEwj2mq_y757oAhXOvJ4KHV22D1EQ_AUoAnoECAwQBA).  批量采购，价格会低于20美元（译者注：1688上的零售价格为148元）.  
  * 替换设备: 测试一个[12v充气泵](https://www.amazon.com/gp/product/B013UQ0T2Y/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) 这个更容易找到（译者注：这个噪音会比较大，但是价格便宜很多，淘宝上20元就能买到，可靠性估计会比较差，用来做测试或许是可以的）.  
  * 替代选择: 3D打印一个鼓风机（译者注：这并不是一个明智的选择，3D打印部件精度很差，价格也很高，不适用此场景） [[讨论]](https://github.com/jcl5m1/ventilator/issues/8)

2.  [Arduino兼容开发板](https://www.amazon.com/s?k=Arduino+nano) 用来控制电机转速, 呼吸循环, 并且处理输入.   Download the [Arduino IDE](https://www.arduino.cc/en/main/software) to program the [microcontroller software](https://github.com/jcl5m1/ventilator/tree/master/ventilator_control).

3. 无刷电机 [电子调速器](https://www.amazon.com/Hobbypower-Brushless-Controller-Multicopter-Helicopter/dp/B00XKX5TBE/ref=sr_1_17?keywords=12v+ESC&qid=1584357758&sr=8-17) 至少要能够承载10A电流. 

4. 用于输入控制的按钮或开关。代码循环通过5级压力。双击可在CPAP和BiPAP/Fixed PEEP模式之间切换.

5. 12v直流电源，至少可以提供5A电流。鼓风机负载很高，呼吸循环可能会导致电压下降，如果电源功率不够，Arduino就会复位。

6. 管道及面罩.  如果你搜索 [CPAP face mask](https://www.google.com/search?q=cpap+mask), 你能发现很多供应商和相关设备.  一个覆盖嘴和鼻子的完整的面罩会使肺部的压力积聚。另一种选择，见下面的草案3D打印部分。

7. 可选的 [24V在线后备电源](https://www.amazon.com/gp/product/B07H8F5HYJ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1).

# 建造过程
这是一个包括面罩、管道、气泵、12V电池、开关和输入的完整系统。 但我强烈建议你使用直流电源而不是电池，因为电池最多能维持3-4个小时。 <strong>电池缺电时使用面罩会导致二氧化碳聚集，这会产生危险.</strong>  这种 [专用电池](https://www.amazon.com/gp/product/B07H8F5HYJ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) 可以边充电边使用, 可以作为墙面电源的后备电源（译者注：万能的淘宝应当有更多可选方案）.

![完整系统图片](https://github.com/jcl5m1/ventilator/blob/master/images/full%20system.jpg?raw=true)

下面是一个鼓风机的特写.  它只是一个直流无刷电机驱动的鼓风机风扇。  上面连接了一个电子调速器和一个Arduino开发板（Teensy2.0++版本，但是目前代码迁移到了Arduino Nano上面）。它有一个3d打印锥形软管适配器，可以配合软管使用。  [微控制器软件](https://github.com/jcl5m1/ventilator/tree/master/ventilator_control) 可以使用 [Arduino IDE](https://www.arduino.cc/en/main/software)进行编程. 软件通过一个简短的初始化序列来配置ESC; 然后从最低的CPAP设置开始工作.  您可以使用开关循环选择通气压力水平，并双击循环选择通气工作模式。

![CPAP 鼓风机](https://github.com/jcl5m1/ventilator/blob/master/images/IMG_20200315_230153.jpg?raw=true)

这是是电子原理图。正如您所看到的，它非常简单，只有很少的几个部件。这是一个轻度修改版本，可以 [感知呼吸循环](https://github.com/jcl5m1/ventilator/wiki/Breathing-Back-Pressure-Data-Analysis).
![schematic](https://github.com/jcl5m1/ventilator/blob/master/images/schematic_20200317.1.jpg?raw=true)


## 面罩 / 管道适配器
因为我有一个CPAP, 这样我就正好可以获得一个[Resmed AitFit F20](https://www.amazon.com/Resmed-AirFit-Frame-System-Cushion/dp/B07C9MR5RS)可以使用的面罩.  它很舒适，并且可以在覆盖口鼻的情况下密封得很好。如果你手头没有,  下面是一个可以使用的方案。我用了一些 [松紧带](https://www.amazon.com/gp/product/B07WZRZDPF/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) 来固定面罩。如果要获得足够的气密性，你需要一些弹力更强的东西。一点点的泄漏实际上是可以接受的，可以让二氧化碳从嘴和鼻子附近逸出，随着时间的推移把空气冲出去; 这样也可以阻止二氧化碳滞留在管道中。  <strong>警告：在断电的情况下使用密封的面罩可导致二氧化碳聚集而产生危险！</strong>

下载3D模型 [[3D model]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/mouthgaurd_v20200316.2.stl) [[Fusion 360 link]](https://a360.co/33rwb1R).

![护口器](https://github.com/jcl5m1/ventilator/blob/master/images/mouthguard.jpg?raw=true)
![Mouth Guard model](https://raw.githubusercontent.com/jcl5m1/ventilator/67c2725fc48a3bc147430cb8c9974f961ff96b7c/images/mouth_guard_model.JPG)


# 压力测试
这是我用来测量输出压力的试验台的图片。它是一个u形管，带有测量带，用来测量水的排水量。 实际的液体位移是测量线的2倍，因为液体在U的另一边被向下推了相同的量，使位移增加了一倍。(I think this is the correct way to measure).  在12v时开足马力, 通气量是 45cmh2o. <strong>[WARNING: 高于 20cmh2o 会有危险](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist)</strong>.  所以这个鼓风机的动力是非常足够的。

![压力测量装置](https://github.com/jcl5m1/ventilator/blob/master/images/test_fixture.jpg?raw=true)

这里有一些图片显示了液体在不同速度下的表现。我手头正好有瓶饮料，相对于白水，这让我更容易看清液位。

![3cm](https://github.com/jcl5m1/ventilator/blob/master/images/3cm.jpg?raw=true) ![6cm](https://github.com/jcl5m1/ventilator/blob/master/images/6cm.jpg?raw=true) ![11cm](https://github.com/jcl5m1/ventilator/blob/master/images/11cm.jpg?raw=true) ![22.5cm](https://github.com/jcl5m1/ventilator/blob/master/images/22.5.jpg?raw=true)

[这是一段鼓风机推动呼吸循环的视频，呼吸循环为16周期/分钟，在12到22cmh2o之间波动](https://photos.app.goo.gl/b3yMPE5QpdeduxKS6).

# 空气过滤 - PAPR 选项

将空气直接灌到某人的气道并不是好主意。如有可能，预先将空气过滤。  这些部件原本是用来DIY PAPR的[Powered Air Purifying Respriator (PAPR)](https://en.wikipedia.org/wiki/Powered_air-purifying_respirator)。不过，加上一个过滤器会显著影响输出气压。这取决于你的马达在额外压力如何工作。  考虑到我测试的鼓风机的净空高度，这些CPAP鼓风机可以在通过过滤器的情况侠仍然达到目标压力。然而，我还没有在高压和更强的过滤器环境下做长时间测试。特别是适配器用了一些胶带和胶水来做密封。 我的鼓风机外壳不是气密的，所以很难保证100%的空气是通过过滤器的。 将鼓风机设置为低CPAP压力，并将面罩通气孔打开，将使其作为PAPR正常工作。

* 这是 [3M P100 or N95 面罩滤芯](https://www.amazon.com/3M-50051138464658-Cartridge-Filter-Organic/dp/B07571LR2K/ref=sr_1_2?crid=36AKE548EW15U&keywords=3m+p100+cartridge&qid=1584418326&sprefix=3m+p100+cartrige%2Caps%2C202&sr=8-2)的转接器。 下载 [[3D 模型]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/3M_filter_adapter.stl) [[Fusion 360 link]](https://a360.co/2QnQQOU)


![3M Apart](https://github.com/jcl5m1/ventilator/blob/master/images/3m_apart.jpg?raw=true) ![3M attached](https://github.com/jcl5m1/ventilator/blob/master/images/3m_attached.jpg?raw=true)

* 这是一个[NATO 40mm gas mask filter cartridge](https://www.amazon.com/MIRA-Cartridge-Respiratory-Protection-Filter/dp/B07L38TYSF/ref=sr_1_2?keywords=40mm+gas+mask+filters&qid=1584418565&sr=8-2)的转接器。  这些过滤器具有These fitlers are available with [CBRN](https://en.wikipedia.org/wiki/CBRN_defense)评级，可作为生化防护使用，类似 [CDC/NIOSH 认可的产品](https://www.cdc.gov/niosh/npptl/standardsdev/cbrn/papr/default.html). 下载 [[3D 模型]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/NATO_40mm_adapter.stl) [[Fusion 360 link]](https://a360.co/3914gXs)



![NATO 部件](https://github.com/jcl5m1/ventilator/blob/master/images/NATO_apart.jpg?raw=true) ![NATO 附件](https://github.com/jcl5m1/ventilator/blob/master/images/NATO_attached.jpg?raw=true)

* 这是一个可选的[内联过滤器](https://www.directhomemedical.com/cart/merchant.mvc?Screen=PROD&Product_Code=1-H1605-inline-bacterial-viral-cpap-filters&Store_Code=DHM&gclid=EAIaIQobChMIo-G35omi6AIVSrzACh29hwv3EAQYASABEgK9FPD_BwE) [[相关讨论]](https://github.com/jcl5m1/ventilator/issues/4)看起来易于安装并且可以在非CPAP鼓风机中使用。 

# 更新日志

点击[这里](https://github.com/jcl5m1/ventilator/wiki) 查看日志。
