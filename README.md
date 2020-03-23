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

# （未完待续）

# To Do's (aka. things I could use help with):
 * I had a long conversation with a pulmonologist to discuss the critical features of a proper ventilator and trade offs. [Here are my notes](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist).  If you know someone with domain expertise, I would like confirmation that my take away notes are reasonable since this will drive priorities on engineering effort/conversations.
 * Develop a simple low-cost sensor configuration that can [provide a similar approximation of lung compliance provided by a ventilator loop display](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist#at-a-high-level-the-goal-is-to-get-enough-air-into-the-lungs-to-keep-the-patient-alive-without-causing-unnecessary-stress-on-infected-lung-tissue)
 * A 3D model for an [inline air filter](https://www.directhomemedical.com/cart/merchant.mvc?Screen=PROD&Product_Code=1-H1605-inline-bacterial-viral-cpap-filters&Store_Code=DHM&gclid=EAIaIQobChMIo-G35omi6AIVSrzACh29hwv3EAQYASABEgK9FPD_BwE) with link to common filter supply [such as this](https://www.amazon.com/3M-Particulate-Filter-Organic-Filters/dp/B079X5C3QP/ref=sr_1_2?keywords=p100+air+filter&qid=1584469511&sr=8-2).
 * Test lung sourcing/research.  Example high end one from [Michigan Instruments](https://www.michiganinstruments.com/lung-simulators/adult-test-lung-simulators/).
 * Alarms for out of target (too low, too high) or out of target range flow/volume.
* A supply chain person that can help us find good suppliers of parts, if there is desire to make these. I don't have a supply chain setup. The few parts I have on hand may not be easily sourcable in any volume quickly.
 * Figure out how to reprogram an existing BiPAP. If this operating mode is helpful, there's a large number of these devices already in the field which could be enabled.  I don't have good stats on the popularity of different makes/models.  There could be on the order of a [1M devices](https://www.cheapcpapsupplies.com/blog/sleep-apnea-statistics/) worldwide?
 * Design modifications to recapture exhaust to minimze addition viral spread. This only works in already "dirty" environments, where there is likely already airborne droplets containing virus - such as quarnateened spaces or other negative air pressure environments.
 * Develop Arduino compatible algorithms to align blower cycle to the breathing cycle by [looking at backpressure load on the blower](https://github.com/jcl5m1/ventilator/wiki/Breathing-Back-Pressure-Data-Analysis), or very simple air pressure sensor that can be inserted into the output of the pump.  For ease of developing algorithms see [Colab notebook with data visualization.](https://colab.research.google.com/drive/1iFMmMMrg_3OeifzJikT75fy4ev84W235)
 * Solutions to prevent the system from becoming unsafe if power is lost.  It's not obvious to me on how to do this.  Ideas are welcome.
 * Test with a [simple inflator pump](https://www.amazon.com/gp/product/B013UQ0T2Y/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) and achieve the same pressure control.
 * Develop a low-cost simple minute volume sensor/approximator.  Here is some information about the [downsides of being over/under on target volume](https://www.acepnow.com/article/avoid-airway-catastrophes-extremes-minute-ventilation/).  Critical care seems to want up to 10-12L/Min.

To provide comments/feedback/offer help, [create a new issue](https://github.com/jcl5m1/ventilator/issues) on the project.  Thanks!


# Useful References/Docs about the supply shortages, and guidance around unapproved devices:

There is a growing list of useful documents around guidance for use of unapproved equipment, and information around estimated shortages of both ventilators and personal protective equipment.  We have moved them to [References Wiki to enable better updates](https://github.com/jcl5m1/ventilator/wiki/Useful-References) to make it easier to maintain.

# Materials
1. [Continuous Positive Airway Pressure (CPAP)](https://en.wikipedia.org/wiki/Continuous_positive_airway_pressure) devices are commonly used by individuals to treat [sleep apnea](https://en.wikipedia.org/wiki/Sleep_apnea). As a result, CPAP blower components are fairly abundant. Used ones are available on eBay and new ones on Alibaba. In many of these devices, the blower is a simple BLDC motor that can be driven with an Electronics Speed Controller (ESC) used by quadrotors and RC cars.  The one I used is pulled from a [Respironics REMStar](https://www.google.com/search?q=respironics+remstar&safe=off&rlz=1C1CHBF_enUS809US809&sxsrf=ALeKk00Uw98vXCAyCiiSglgt-2Ucnz5RCg:1584357572342&source=lnms&tbm=isch&sa=X&ved=2ahUKEwj2mq_y757oAhXOvJ4KHV22D1EQ_AUoAnoECAwQBA).  In volume, these blower components can be under $20.  
  * Alternative: test a [12v inflator pump](https://www.amazon.com/gp/product/B013UQ0T2Y/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) which is even more abundant.  
  * Alternative: [print a blower](https://drmrehorst.blogspot.com/2018/04/the-mother-of-all-print-cooling-fans.html) [[discussion]](https://github.com/jcl5m1/ventilator/issues/8)

2.  [Arduino Compatible Nano/Clone](https://www.amazon.com/s?k=Arduino+nano) to control the motor speed, breathing cycles, and handle user input.   Download the [Arduino IDE](https://www.arduino.cc/en/main/software) to program the [microcontroller software](https://github.com/jcl5m1/ventilator/tree/master/ventilator_control).

3. Brushless DC Motor [Electronic Speed Controller](https://www.amazon.com/Hobbypower-Brushless-Controller-Multicopter-Helicopter/dp/B00XKX5TBE/ref=sr_1_17?keywords=12v+ESC&qid=1584357758&sr=8-17) capable of at least 10A. 

4. Button or switch for input control.  The code cycles through 5 levels of pressure. Double click to switch between CPAP and BiPAP/Fixed PEEP mode.

5. 12v DC power supply that can handle at least 5A.  The blower works pretty hard, and the breathing cycles can create voltage drops which will reset the Arduino if the supply is not strong enough.

6. Tubing and face mask.  If you search for [CPAP face mask](https://www.google.com/search?q=cpap+mask), you'll find many options/suppliers.  A full face mask that covers both the mouth and nose will enable pressure buildup in the lungs.  As an alternative, see below for draft 3D printable parts.

7. Optional [inline 12v battery backup](https://www.amazon.com/gp/product/B07H8F5HYJ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1).

# Building
This is the full system with mask, tubing, pump, 12v battery, and switch for input.  However, I would strongly recommend running this with a DC power supply since the battery will only last about 3-4 hours.  <strong>Wearing the mask with a dead battery could cause dangerous CO2 build up.</strong>  This [particular battery](https://www.amazon.com/gp/product/B07H8F5HYJ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) can charge and supply power at the same time, acting as an inline battery backup to wall power.

![Full System](https://github.com/jcl5m1/ventilator/blob/master/images/full%20system.jpg?raw=true)

Below is a close up of the extracted blower.  It is simply a BLDC motor driving a blower fan.  A small ESC and Arduino are attached (technically a Teensy2.0++, but the code has now been changed to an Arduino Nano).  It has a 3d printed tapered hose adpater on it to fit in the hose.  The [microcontroller software](https://github.com/jcl5m1/ventilator/tree/master/ventilator_control) can be programmed with the [Arduino IDE](https://www.arduino.cc/en/main/software). The software goes through a short initialization sequence to configure the ESC; it then starts at the lowest CPAP setting.  You can use the switch to cycle through pressure levels, and double click to cycle through operating modes.

![Extracted CPAP Blower](https://github.com/jcl5m1/ventilator/blob/master/images/IMG_20200315_230153.jpg?raw=true)

Here is the schematic for the electronics. As you can see, it is very simple with only a few parts.  A slightly modifed version that is able to [sense the blower current is here](https://github.com/jcl5m1/ventilator/wiki/Breathing-Back-Pressure-Data-Analysis).
![schematic](https://github.com/jcl5m1/ventilator/blob/master/images/schematic_20200317.1.jpg?raw=true)


## Face mask / Tube Adapter
Since I have a CPAP, I happen to have a [Resmed AitFit F20](https://www.amazon.com/Resmed-AirFit-Frame-System-Cushion/dp/B07C9MR5RS) mask that I can use.  This is quite comfortable and covers both the nose and mouth to make a good seal.  However, if you can't get a mask,  below is a prototype mouthguard that fits in the category of not-so-great-but-usable-if-you-have-a-lot-of-tape.  I am using some [elastic straps](https://www.amazon.com/gp/product/B07WZRZDPF/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) as head gear.  However, in order to get a good air seal to get enough positive pressure, this would require some tape.  A little bit of leakage is actually desirable to allow CO2 to escape near the mouth and nose to flush out the air over time; this prevents CO2 from being stuck in the tube.  <strong>WARNING: wearing this sealed to the mouth with tape without power may cause dangerous CO2 build up.</strong>

Download the [[3D model]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/mouthgaurd_v20200316.2.stl) [[Fusion 360 link]](https://a360.co/33rwb1R).

![Mouth Guard](https://github.com/jcl5m1/ventilator/blob/master/images/mouthguard.jpg?raw=true)
![Mouth Guard model](https://raw.githubusercontent.com/jcl5m1/ventilator/67c2725fc48a3bc147430cb8c9974f961ff96b7c/images/mouth_guard_model.JPG)


# Pressure Testing

This is a picture of my test rig to measure the output pressure.  It is a U-shaped tube with an attached measuring tape to check displacement of water.  The actual liquid displacement is 2x the measured line since liquid is being pushed downwards an equal amount on the other side of the U, doubling the displacement. (I think this is the correct way to measure).  At full blast at 12v, it is achieving 45cmh2o. <strong>[WARNING: Going above 20cmh2o can be DANGEROUS](https://github.com/jcl5m1/ventilator/wiki/Notes-from-chatting-with-a-pulmonologist)</strong>.  So, these blowers are plently powerful.

![Pressure measurement fixture](https://github.com/jcl5m1/ventilator/blob/master/images/test_fixture.jpg?raw=true)

Here are some images showing the dislacement of the liquid at different speeds.  I happen to have Diet Dr. Pepper on hand which makes it easier to see the liquid level rather than just plain water.

![3cm](https://github.com/jcl5m1/ventilator/blob/master/images/3cm.jpg?raw=true) ![6cm](https://github.com/jcl5m1/ventilator/blob/master/images/6cm.jpg?raw=true) ![11cm](https://github.com/jcl5m1/ventilator/blob/master/images/11cm.jpg?raw=true) ![22.5cm](https://github.com/jcl5m1/ventilator/blob/master/images/22.5.jpg?raw=true)

Here's a [video of the blower pushing a breathing cycle of 16 cycles/min oscilating between 12 and 22cmh2o](https://photos.app.goo.gl/b3yMPE5QpdeduxKS6).

# Air Filtration - PAPR Option

An open air blower into someone's airway isn't great.  If possible, some filtration is preferred.  These parts were originally used for a DIY [Powered Air Purifying Respriator (PAPR)](https://en.wikipedia.org/wiki/Powered_air-purifying_respirator). However, adding a filter will definitely affect the output pressure.  It will depend on the blower you have if the motor can handle the additional load.  Given the headroom of the blower I tested, these CPAP blowers can probably handle the filter and still hit the target pressure.  However, I haven't done long term thermal testing at high pressure and with a strong filter. These adapter plates can be attached with liberal amounts of hot glue and wrapping the unit in vinyl tape to get a reasonably airtight seal.  My blower's enclosure was not air-tight, so it is difficult to guarantee that 100% of the air is coming only through the filter.  Setting the blower to a low CPAP pressure, and leaving the face mask vent holes open will allow it to function reasonably as a PAPR.

* This is an adapter plate for a [3M P100 or N95 face mask filter cartridge](https://www.amazon.com/3M-50051138464658-Cartridge-Filter-Organic/dp/B07571LR2K/ref=sr_1_2?crid=36AKE548EW15U&keywords=3m+p100+cartridge&qid=1584418326&sprefix=3m+p100+cartrige%2Caps%2C202&sr=8-2). Download [[3D model]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/3M_filter_adapter.stl) [[Fusion 360 link]](https://a360.co/2QnQQOU)


![3M Apart](https://github.com/jcl5m1/ventilator/blob/master/images/3m_apart.jpg?raw=true) ![3M attached](https://github.com/jcl5m1/ventilator/blob/master/images/3m_attached.jpg?raw=true)

* This is an adapter plate for a [NATO 40mm gas mask filter cartridge](https://www.amazon.com/MIRA-Cartridge-Respiratory-Protection-Filter/dp/B07L38TYSF/ref=sr_1_2?keywords=40mm+gas+mask+filters&qid=1584418565&sr=8-2).  These fitlers are available with [CBRN](https://en.wikipedia.org/wiki/CBRN_defense) ratings which are needed for viral and bacterial defense similar to those [approved by the CDC/NIOSH](https://www.cdc.gov/niosh/npptl/standardsdev/cbrn/papr/default.html). Download [[3D model]](https://github.com/jcl5m1/ventilator/blob/master/3dmodels/NATO_40mm_adapter.stl) [[Fusion 360 link]](https://a360.co/3914gXs)



![NATO Apart](https://github.com/jcl5m1/ventilator/blob/master/images/NATO_apart.jpg?raw=true) ![NATO attached](https://github.com/jcl5m1/ventilator/blob/master/images/NATO_attached.jpg?raw=true)

* This is an option for an [inline filter](https://www.directhomemedical.com/cart/merchant.mvc?Screen=PROD&Product_Code=1-H1605-inline-bacterial-viral-cpap-filters&Store_Code=DHM&gclid=EAIaIQobChMIo-G35omi6AIVSrzACh29hwv3EAQYASABEgK9FPD_BwE) [[discussion]](https://github.com/jcl5m1/ventilator/issues/4) that looks easy to install, and would be helpful for non-CPAP blowers. 

# Update Log

Click [here](https://github.com/jcl5m1/ventilator/wiki) to see updates.
