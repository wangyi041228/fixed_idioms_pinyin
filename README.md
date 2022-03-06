# handle_src_data_idioms.json
使用汉典数据和某字典数据修复汉兜数据。  
[汉典官网](https://www.zdic.net/)  
[字典数据库](https://github.com/pwxcoo/chinese-xinhua)  
[汉兜数据](https://github.com/antfu/handle/blob/main/src/data/idioms.json)  
## 字典说明
中华新华字典数据库（并非新华字典官方，数据来http://www.zd9999.com，该站已转为影视字典，以下简称字典）收录成语30895条目，其中四字条目29502。汉兜此前的词库29503条目，只多一个`仓颉造字`。字典成语dirty版收录31648个条目，多出的753条目中有26条拼音标注不同（错误、\u表示或标点），其余文字和拼音完全一致。该字典清洗后的数据有大量错误。中文互联网，哎……  
## 对汉兜的建议
像Wordle一样对输入进行检查，没有命中词库直接驳回，可以避免强行为`阿阿阿阿`注音的尴尬场景。  
## 关于变调/同音
拼音标注不考虑变调，按正字标注。(一，不，众三声）  
难兄难弟有2声和4声义项，理应分开，但你懂的，暂只按4声收录。
## 汉典全爬
汉典提供成语部首索引，但搜【事】无结果，暂时搁置。
## 文件说明
`idioms.json`可直接替换原工程对应文件。  
按照原始文件，`ü`一律写作`v`。  
## 汉兜此前收录，但汉典没有的161文字条目，已人工修正24条
【抜格不入】→【扞格不入】抜ba2，扞han4  
【.*鄐诜.*】→【.*郤诜.*】和【.*郄诜.*】（2条变4条）  
【.*痜.*】→【.*疐.*】痜tu1，疐zhi4 di4（5条）  
【前跋后疐】虽然汉典也收录疐mao2，但我没查到这个音。我从不认为汉典数据全对。  
【仓颉造字】暂时保留  
（剔除重复）【宾餿日月】→【宾饯日月】餿sou1繁，饯jian4  
【.*壸.*】→【.*壶.*】壸kun3，壶hu2（6条剔1条为5条）  
【炳炳焤焤】→【炳炳烺烺】焤fu3，烺lang3  
【病入骨雜】→【病入骨随】雜za2繁，随sui2  
【不胜梘杓】→【不胜桮杓】梘jian3繁，桮bei  
【尺壁寸阴】→【尺璧寸阴】  
【大块朵颐】→【大快朵颐】  
（剔除重复）【好高鹜远】→【好高骛远】  
（剔除重复）【.*閒.*】→【.*熔.*】閒xian2jian1jian4，熔rong2（2条）  
（剔除重复）【经帮纬国】→【经邦纬国】  
## 剩余137文字条目还需修正/采纳/剔除
不知藋蕫  
草藄禽猘  
称体载衣  
遫俗绝物  
崇论豠议  
淡汝浓抹  
鼎折覆餸  
鼎折餸覆  
动中竨要  
抖搂精神  
饭囊酒畒  
鲂鱼趙尾  
瞓面盎背  
猦穅及米  
冯髈弹铗  
凤臆龙鬵  
伏而唂天  
妇姑勃豨  
附赘悬胾  
膏梁纨裦  
膏梁子弟  
膏粱纨裦  
号唃大哭  
鸿鷑凤立  
鸿鷑凤逝  
鸿鴆满纸  
花下晒裻  
花枝招飍  
黄干黑廲  
黄皮刮廲  
黄皮寡廲  
混混泇泇  
蹐地踨天  
监市履猯  
骄儿騣女  
截发剉穢  
金鴗擘海  
进退触籵  
狼顾鸱踤  
离蔬释躥  
犁牛髐角  
犁生髐角  
龙踚虎卧  
龙骧虎踤  
邈处歬视  
名韟利鞚  
目攋耳染  
蹑躥担簦  
蹑躥檐簦  
牛农对泣  
旁蒷远绍  
批鄐导竨  
批隙导竨  
批砉导竨  
磇硄混玉  
骈首就僯  
飘籵坠溷  
牝哹鸣辰  
七鄐八手  
气吞虹蝩  
诎要桡膎  
认奴作鄌  
衽抭囊括  
日杒月减  
日杒月削  
日削月杒  
入室昻堂  
三舖八菹  
桑枢畒牖  
山陬海噬  
上焌下报  
虱处裻中  
十夫榪椎  
思断义绝  
死声唃气  
死有余僯  
四海昻平  
遬听远闻  
岁在龙蚮  
遂迷不竝  
贪夫猣财  
贪夫猣利  
天之僯民  
同心僯力  
纨裦膏粱  
纨裦子弟  
望尘僩声  
餵糟啜漓  
餵糟啜醨  
餵糟歠漓  
餵糟歠醨  
乌踷兔走  
无羐无碍  
俠多俠少  
瑕不搑瑜  
鸮心鹺舌  
行色恠恠  
汹涌渒湃  
熊据虎踤  
悬梁刺骨  
悬猙素飡  
宴安醙毒  
晏安醙毒  
燕安醙毒  
扬风抦雅  
摇头穢脑  
摇头黣尾  
依乷附木  
以磛投卵  
瑜不搑瑕  
雨昫时若  
鬻矛誉榡  
渊涓蠖瀋  
沅茞澧兰  
臧穣亡羊  
崭露头脚  
折鼎覆餸  
折足覆餸  
枕黮藉糟  
重裵列鼎  
重气猣名  
朱辬皁盖  
朱辬皂盖  
祝僯祝鲠  
祝鮠之佞  
孜孜砽砽  
孳孳砽砽  
踨地籥天  
踨高蹐厚  
踨蹐不安  
踨天促地  
踨天蹐地  
騣女痴儿  
騣女痴男  
騣童钝夫  
坐地分脏  
## 相同文字但拼音不同，参考汉兜数据和常识对汉典数据进行修复
例如：
片言只zhi1语  
片言只zhi1字  
片语只zhi1辞  
片纸只zhi1字  
坐视shi4不救  
不破po4不立  
赭衣塞se4路  
跌宕风feng1流liu2  
悬龟系鱼  
改行自新  
除`绿林`等少量词汇外的绿lv4  
大da4步流星  
支吾wu2其词  
葬身鱼yu2腹  
约yue1法三章  
语笑喧阗tian2  
与民min2更始  
有隙可乘cheng2  
有加无wu2已  
把玩无wu2厌  
身shen2  
以蠡li2测海  
狸li2  
一五wu3一十  
览lan3  
一yi1  
叶落归gui1根  
蝎蝎螫zhe1螫  
瑕瑜互见xian4  
无可比拟ni3  
无病呻吟yin2  
稳wen3  
首/手shou3  
铤ting3鹿走险  
涕泗滂pang1沱  
身心xin1交病  
上当dang4学乖  
善善恶wu4恶e4  
日居ju1月诸zhu1  
取而er2代之  
情急智zhi4生sheng1  
勤学苦练lian4  
泣qi4不成声  
偏听偏pian1信  
拿刀动dong4杖  
目瞪舌彊jiang4  
谋无遗谞(汉典上半部对，下半部错）  
莫予yu4毒也  
尨pang2眉皓发  
ye
单枪匹pi3马  
颠乾qian2倒坤  
风云变bian4幻  
拱肩jian1缩背  
官运亨通tong1  
不bu4  
欢呼雀que4跃  
简明扼e4要  
进jin4  
雷霆之zhi1怒nu4  
里出外进jin4  
龙吟yin2虎啸  
屡教jiao4不改  
添砖加jia1瓦  
约yue1法三章  
## 存疑
传神阿堵  
## 汉典与汉兜现有拼音对比
| 成语 | 汉典拼音 | 汉兜数据 |
| --- | --- | --- |
| 百花争妍 | bai3 hua1 zheng1 yan2 | bai3 hua1 zheng1 yan4 |
| 鼻塌脣青 | bi2 ta1 chun2 qing1 | bi2 ta3 chun2 qing1 |
| 弊帚自珍 | bi4 zhou3 zi4 zhen1 | bi4 zhou3 zi4 zhen2 |
| 便宜从事 | bian4 yi2 cong2 shi4 | bian2 yu2 cong2 shi4 |
| 便宜施行 | bian4 yi2 shi1 xing2 | bian2 yu2 shi1 xing2 |
| 不破不立 | bu4 puo4 bu4 li4 | bu4 po4 bu4 li4 |
| 惨绿愁红 | can3 lu4 chou2 hong2 | can3 lv4 chou2 hong2 |
| 惨绿少年 | can3 lu4 shao3 nian2 | can3 lv4 shao4 nian2 |
| 苍白无力 | cang1 bai2 bui2 li4 | ang1 bai2 bui2 li4 |
| 层见错出 | ceng2 xian4 cuo4 chu1 | ceng2 chu1 cuo4 jian4 |
| 成家立业 | cheng2 jia1 li4 yie4 | cheng2 jia1 li4 ye4 |
| 愁红惨绿 | chou2 hong2 can3 lu4 | chou2 hong2 can3 lv4 |
| 愁眉不展 | chou2 mei2 bu4 zhan1 | chou2 mei2 bu4 zhan3 |
| 传风搧火 | chuan2 feng1 shan1 huo3 | chuan2 feng1 you3 huo3 |
| 传神阿堵 | chuan2 shen2 a1 du3 | chuan2 shen2 e1 du3 |
| 歠菽饮水 | chuo4 shu1 yin3 shui3 | pa2 shu1 yin3 shui3 |
| 大步流星 | da3 bu4 liu2 xing1 | da4 bu4 liu2 xing1 |
| 大大落落 | da4 da luo1 luo1 | da4 da4 luo4 luo4 |
| 大雨滂沱 | da4 yu3 pang1 tuo2 | da4 yu3 pang2 tuo2 |
| 单枪匹马 | dan1 qiang1 pi2 ma3 | dan1 qiang1 pi3 ma3 |
| 颠乾倒坤 | dian1 qian1 dao3 kun1 | dian1 qian2 dao3 kun1 |
| 跌宕风流 | die1 dang4 fengliu12 | die1 dang4 feng liu2 |
| 冬箑夏裘 | dong1 sha4 xia4 qiu2 | dong1 zha2 xia4 qiu2 |
| 斗筲穿窬 | dou3 shao1 chuan1 yu2 | dou4 shao1 chuan1 yu2 |
| 笃近举远 | du3 jin4 ju3 yuan3 | du3 jin4 ju3 juan3 |
| 额首称庆 | e2 shou3 cheng1 qing4 | e2 shou1 cheng1 qing4 |
| 发怒冲冠 | fa4 nu4 chong1 guan1 | fa1 nu4 chong1 guan4 |
| 发上冲冠 | fa4 shang4 chong1 guan1 | fa1 shang4 chong1 guan4 |
| 发上指冠 | fa4 shang4 zhi3 guan1 | fa1 shang4 zhi3 guan4 |
| 风尘肮脏 | feng1 chen2 ang1 zang1 | feng chen ang zang |
| 风云变幻 | feng1 yun2 bia4 huan4 | feng1 yun2 bian4 huan4 |
| 风姿绰约 | feng1 zi1 chuo4 yue1 | feng1 zi1 chuo1 yue2 |
| 负债累累 | fu4 zhai4 lei3 lei3 | fu4 zhai lei4 lei4 |
| 改行自新 | gai3 xing2 zixin41 | gai3 xing2 zi4 xin1 |
| 葛屦履霜 | ge2 ju4 lv3 shuang1 | ge3 ju4 lv3 shuang1 |
| 各有所长 | ge4 you3 suo3 chang2 | ge4 you3 suo3 cheng2 |
| 攻城掠地 | gong1 cheng2 lve4 di4 | gong1 cheng2 lve3 di4 |
| 拱肩缩背 | gong3 jan1 suo1 bei4 | gong3 jian1 suo1 bei4 |
| 古肥今瘠 | gu3 fei2 jin1 ji2 | gu3 fei2 jin1 shou4 |
| 瓜葛相连 | gua1 ge2 xiang1 lian2 | gua1 ge3 xiang1 lian2 |
| 官运亨通 | guan1 yun4 heng1 gong1 | guan1 yun4 heng1 tong1 |
| 过都历块 | guo4 du1 li4 kuai4 | guo4 dou1 li4 kuai4 |
| 蒿目时艰 | hao1 mu4 shi2 jian1 | hang4 mu4 shi2 jian1 |
| 划粥割齑 | hua4 zhou1 ge1 ji1 | hua4 zhou1 ge1 jiu1 |
| 怀才不遇 | huai2 cai2 bu1 yu4 | huai2 cai2 bu4 yu4 |
| 怀柔天下 | huai2 rou2 tian1 xia4 | huai rou tian xia |
| 欢呼雀跃 | huan1 hu1 que2 yue2 | huan1 hu1 que4 yue4 |
| 鹡鸰在原 | ji2 ling2 zai4 yuan2 | xia4 ling2 zai4 yuan2 |
| 戟指怒目 | ji3 zhi3 nu3 mu4 | ji3 zhi3 nu3 zhang1 |
| 坚壁清野 | jian1 bi4 qing1 yie3 | jian1 bi4 qing1 ye3 |
| 间不容发 | jian1 bu4 rong2 fa4 | jian4 bu4 rong2 fa4 |
| 间不容瞚 | jian1 bu4 rong2 shun4 | jian1 bu4 rong2 xi3 |
| 简明扼要 | jian3 ming2 e2 yao4 | jian3 ming2 e4 yao4 |
| 诘屈磝碻 | ji2 qu1 ao2 qiao1 | jie2 qu1 bing4 zhou4 |
| 诘屈謷牙 | ji2 qu1 ao2 ya2 | jie2 qu1 da4 ya2 |
| 戒奢宁俭 | jie4 she1 ning4 jian1 | jie4 she1 ning4 jian3 |
| 进退两难 | jin3 tui4 liang3 nan2 | jin4 tui4 liang3 nan2 |
| 九蒸三熯 | jiu3 zheng1 san1 han4 | jiu3 zheng1 san1 sheng1 |
| 君子好逑 | jun1 zi3 hao3 qiu2 | jun1 zi3 hao4 qiu2 |
| 坑蒙拐骗 | keng1 meng1 guai3 pian4 | keng1 meng2 guai3 pian4 |
| 款曲周至 | kuan3 qu1 zhou1 zhi4 | kuan3 qu3 zhou1 zhi4 |
| 锒铛入狱 | lang2 dang1 ru4 yu4 | lang2 kang1 ru4 yu4 |
| 唠唠叨叨 | lao2 lao dao1 dao1 | lao1 lao1 dao1 dao1 |
| 雷霆之怒 | lei2 ting2 wan4 j | lei2 ting2 zhi1 nu4 |
| 里出外进 | li3 chu1 wai4 lian2 | li3 chu1 wai4 jin4 |
| 力有未逮 | li4 you3 wei4 dai4 | li4 you3 wei4 dai3 |
| 龙吟虎啸 | long2 yin1 hu3 xiao4 | long2 yin2 hu3 xiao4 |
| 露红烟绿 | lu4 hong2 yan1 lu4 | lu4 hong2 yan1 lv4 |
| 屡教不改 | lv3 jian4 bu4 gai3 | lv3 jiao4 bu4 gai3 |
| 率尔操觚 | shuai4 er3 cao1 gu1 | shuai4 er2 cao1 gu1 |
| 尨眉皓发 | manɡ2 mei2 hao4 fa4 | chou2 mei2 hao4 fa1 |
| 毛遂自荐 | mao2 sui4 zi4 jian4 | mao2 sui2 zi4 jian4 |
| 莫予毒也 | mo4 yu4 du2 ye3 | mo4 yu2 du2 ye3 |
| 谋无遗谞 | mou2 wu2 yi2 xu1 | mou2 wu2 yi2 er2 |
| 目瞪舌彊 | mu4 deng4 she2 qiang2 | mu4 deng4 she2 jiang4 |
| 拿刀动杖 | na2 dao1 nong4 zhang4 | na2 dao1 dong4 zhang4 |
| 内圣外王 | nei4 sheng4 wai4 wang2 | nei4 sheng4 wai4 zhu3 |
| 逆行倒施 | ni4 xing2 dao4 shi1 | ni4 xing2 dao3 shi1 |
| 年高德卲 | nian2 gao1 de2 shao4 | nian2 gao1 de2 er2 |
| 滂沱大雨 | pang1 tuo2 da4 yu3 | pang2 tuo2 da4 yu3 |
| 批亢捣虚 | pi1 kang4 dao3 xu1 | pi1 gang4 dao3 xu1 |
| 片言只语 | pian4 yan2 zhi3 yu3 | pian4 yan2 zhi1 yu3 |
| 片语只辞 | pian4 yan2 zhi3 ci2 | pian4 yu3 zhi3 ci2 |
| 片纸只字 | pian4 zhi3 yan2 zi4 | pian4 zhi3 zhi1 zi4 |
| 偏听偏信 | pian1 ting1 piang1 xin4 | pian1 ting1 pian1 xin4 |
| 帡天极地 | pinɡ2 tian1 ji2 di4 | ju2 tian1 ji2 di4 |
| 破璧毁珪 | po4 bi4 hui3 ɡui1 | po4 bi4 hui3 zhi3 |
| 破斧缺斨 | po4 fu3 que1 qiang1 | po4 fu3 que1 zhou1 |
| 泣不成声 | qi3 bu4 cheng2 sheng1 | qi4 bu4 cheng2 sheng1 |
| 强弓劲弩 | qiang2 gong1 jing4 nu3 | qiang2 gong1 jin4 nu3 |
| 勤学苦练 | qin2 xue2 ku3 zh | qin2 xue2 ku3 lian4 |
| 擒奸擿伏 | qin2 jian1 ti1 fu2 | qin2 jian1 fa1 fu2 |
| 情急智生 | qing2 ji2 sheng1 zhi4 | qing2 ji2 zhi4 sheng1 |
| 曲肱而枕 | qu1 gong1 er2 zhen3 | qu3 gong1 er2 zhen3 |
| 取而代之 | qu3 e2 dai4 zhi1 | qu3 er2 dai4 zhi1 |
| 忍俊不禁 | ren3 jun4 bu4 jin1 | ren3 jun4 bu4 jin4 |
| 日居月诸 | ri4 ji1 yue4 zh | ri4 ju1 yue4 zhu1 |
| 三年五载 | san1 nian2 wu3 zai3 | san1 nian2 wu3 zai4 |
| 丧胆销魂 | sang4 dan3 xiao1 hun2 | sang4 hun2 xiao1 hun2 |
| 善善恶恶 | shan4 shan4 e4 e4 | shan4 shan4 wu4 e4 |
| 上当学乖 | shang4 dang1 xue2 guai1 | shang4 dang4 xue2 guai1 |
| 身心交病 | shen1 xing1 jiao1 bing4 | shen1 xin1 jiao1 bing4 |
| 神魂荡飏 | shen2 hun2 dang4 yang2 | shen2 hun2 dang4 chen2 |
| 鼪鼯之径 | sheng1 wu2 zhi1 jing4 | wei2 wu2 zhi1 jing4 |
| 鼪鼬之迳 | sheng1 you4 zhi1 jing4 | tian1 you4 zhi1 jing4 |
| 瘦骨嶙峋 | shou4 gu3 lin2 xun2 | shou4 gu3 li2 xun2 |
| 书声琅琅 | shu1 sheng1 lang2 lang2 | shu1 sheng1 lang3 lang3 |
| 薮中荆曲 | sou3 zhong1 jing1 qu3 | sou3 zhong1 ji2 qu3 |
| 涕泗滂沱 | ti4 si4 pang2 tuo2 | ti4 si4 pang1 tuo2 |
| 添砖加瓦 | tian1 zhuan1 jie1 wa3 | tian1 zhuan1 jia1 wa3 |
| 靦颜人世 | mian3 yan2 ren2 shi4 | tian3 yan2 ren2 shi4 |
| 铤鹿走险 | ding4 lu4 zou3 xian3 | ting3 lu4 zou3 xian3 |
| 玩岁愒月 | wan2 sui4 kai4 yue4 | wan2 sui4 yi1 yue4 |
| 汪洋自恣 | wang1 yang2 zi4 zi4 | wang1 yang2 zi4 zi1 |
| 畏首畏尾 | wei4 sho3 wei4 wei3 | wei4 shou3 wei4 wei3 |
| 稳操胜券 | wen2 cao1 sheng4 quan4 | wen3 cao1 sheng4 quan4 |
| 无病呻吟 | wu2 bing4 shen1 yin1 | wu2 bing4 shen1 yin2 |
| 无可比拟 | wu2 ke3 bi3 ni4 | wu2 ke3 bi3 ni3 |
| 物阜民安 | wu4 fu4 min2 an1 | wu4 fu3 min2 an1 |
| 物竞天择 | wu4 jing4 tian1 ze2 | wu4 jin4 tian1 ze2 |
| 物美价廉 | wu4 mei3 jia4 lian2 | jia4 lian2 wu4 mei3 |
| 瑕瑜互见 | xia2 yu2 hu4 jian4 | xia2 yu2 hu4 xian4 |
| 咸阳一炬 | xian2 yang2 yi1 ju4 | xian2 yang2 yi1 ju3 |
| 挦毛捣鬓 | xian2 mao2 dao3 bin4 | tun2 mao2 dao3 bin4 |
| 挦绵扯絮 | xian2 mian2 che3 xu4 | chan2 mian2 che3 xu4 |
| 挦章撦句 | xian2 zhang1 zong1 ju4 | long2 zhang1 zong1 ju4 |
| 枵腹终朝 | xiao1 fu4 zhong1 zhao1 | xiao1 fu4 zhong1 chao2 |
| 鸮鸣鼠暴 | xiao1 ming2 shu3 bao4 | zhang1 ming2 shu3 bao4 |
| 鸮鸟生翼 | xiao1 niao3 sheng1 yi4 | qing1 niao3 sheng1 yi4 |
| 鸮啼鬼啸 | xiao1 ti2 gui3 xiao4 | niao3 ti2 gui3 xiao4 |
| 鸮心鹂舌 | xiao1 xin1 li2 she2 | ren2 xin1 li2 she2 |
| 蝎蝎螫螫 | xie1 xie1 zhe2 zhe2 | xie1 xie1 zhe1 zhe1 |
| 挟势弄权 | xie2 shi4 nong4 quan2 | jia1 shi4 nong4 quan2 |
| 悬龟系鱼 | xuan2 guiji14 yu2 | xuan2 gui ji4 yu2 |
| 叶落归根 | ye4 luo4 hui1 gen1 | ye4 luo4 gui1 gen1 |
| 一板一眼 | yi1 ban3 yin1 yan3 | yi1 ban3 yi1 yan3 |
| 一哄而散 | yi1 honɡ4 er2 san4 | yi1 hong4 er2 san4 |
| 一哄而上 | yi4 hong1 er2 shang4 | yi1 hong1 er2 shang4 |
| 一览无余 | yi1 lai3 wu2 yu2 | yi1 lan3 wu2 yu2 |
| 一邱之貉 | yi1 qiu1 zhi1 he2 | yi1 qiu1 zhi1 he4 |
| 一五一十 | yi1 wu2 yi1 shi2 | yi1 wu3 yi1 shi2 |
| 移宫换羽 | yi2 gong1 huan4 yu3 | yi2 dong1 huan4 yu3 |
| 以蠡测海 | yi3 li3 ce4 hai3 | yi3 li2 ce4 hai3 |
| 以身报国 | yi3 sheng1 bao4 guo2 | yi3 shen1 bao4 guo2 |
| 以身许国 | yi3 sheng1 xu3 guo2 | yi3 shen1 xu3 guo2 |
| 以身殉国 | yi3 sheng1 xun4 guo2 | yi3 shen1 xun4 guo2 |
| 以噎废飡 | yi3 ye1 fei4 can1 | yi3 ye1 fei4 guang1 |
| 喑噁叱咤 | yin1 e4 chi4 zha4 | yin1 wu4 chi4 zha4 |
| 淫言媟语 | yin2 yan2 xie4 yu3 | yin2 yan2 liang3 yu3 |
| 永永无穷 | yong3 yong3 wu2 qiong2 | yong3 shi4 wu2 qiong2 |
| 用行舍藏 | yong4 xing2 she3 cang2 | yong4 xing2 cang2 she3 |
| 有加无已 | you3 jia1 wu3 yi3 | you3 jia1 wu2 yi3 |
| 有隙可乘 | you3 xi4 ke3 cheng4 | you3 xi4 ke3 cheng2 |
| 杅穿皮蠹 | yu2 chuan1 pi2 du4 | yu2 chuan1 shui3 du4 |
| 与民更始 | yu3 ren2 geng1 shi3 | yu3 min2 geng1 shi3 |
| 语笑喧阗 | yu3 xiao4 xuan1 tian1 | yu3 xiao4 xuan1 tian2 |
| 约法三章 | yue4 fa3 san1 zhang1 | yue1 fa3 san1 zhang1 |
| 葬身鱼腹 | zang4 shen1 yu1 fu4 | zang4 shen1 yu2 fu4 |
| 乍暖还寒 | zha4 nuan3 huan2 han2 | zha4 nuan3 hai2 han2 |
| 赭衣塞路 | zhe3 yi1 sai41 lu4 | zhe3 yi1 se4 lu4 |
| 支吾其词 | zhi1 wu1 qi2 ci2 | zhi1 wu2 qi2 ci2 |
| 指囷相赠 | zhi3 qun1 xiang1 zeng4 | zhi3 que4 xiang1 zeng4 |
| 装模作样 | zhuang1 mu2 zuo4 yang4 | zhuang1 mo2 zuo4 yang4 |
| 坐视不救 | zuo4 shi1 bu4 jiu4 | zuo4 shi4 bu4 jiu4 |
## 汉典（上半部）与字典拼音对比
| 成语 | 汉典拼音 | 字典拼音 |
| --- | --- | --- |
| 昂藏七尺 | ang2 cang2 qi1 chi3 | ang2 zang4 qi1 chi3 |
| 百花争妍 | bai3 hua1 zheng1 yan2 | bai3 hua1 zheng1 yan4 |
| 鼻塌脣青 | bi2 ta1 chun2 qing1 | bi2 ta3 chun2 qing1 |
| 弊帚自珍 | bi4 zhou3 zi4 zhen1 | bi4 zhou3 zi4 zhen2 |
| 鞭辟近里 | bian1 pi4 jin4 li3 | bian1 bi4 jin4 li3 |
| 便宜从事 | bian4 yi2 cong2 shi4 | bian2 yu2 cong2 shi4 |
| 便宜施行 | bian4 yi2 shi1 xing2 | bian2 yu2 shi1 xing2 |
| 便宜行事 | bian4 yi2 xing2 shi4 | bian4 yi4 xing2 shi4 |
| 惨绿愁红 | can3 lu4 chou2 hong2 | can3 lü chou2 hong2 |
| 惨绿年华 | can3 lu4 nian2 hua2 | can3 lü4 nian2 hua2 |
| 惨绿少年 | can3 lu4 shao3 nian2 | can3 lü4 shao4 nian2 |
| 苍白无力 | cang1 bai2 bui2 li4 | ang1 bai2 bui2 li4 |
| 层见错出 | ceng2 xian4 cuo4 chu1 | ceng2 chu1 cuo4 jian4 |
| 层见叠出 | ceng2 xian4 die2 chu1 | ceng2 jian4 die2 chu1 |
| 长幼有序 | zhang3 you4 you3 xu4 | zhang　you　you　xu3434 |
| 沉厚寡言 | chen2 hou4 gua3 yan2 | chen　hou　gua　yan2432 |
| 沉重寡言 | chen2 zhong4 gua3 yan2 | chen　zhong　gua　yan2432 |
| 沉著痛快 | chen2 zhuo2 tong4 kuai4 | chen2 zhu4 tong4 kuai4 |
| 愁红惨绿 | chou2 hong2 can3 lu4 | chou2 hong2 can3 lü |
| 穿红着绿 | chuan1 hong2 zhe lu4 | chuan1 hong2 zhuo2 lü4 |
| 传风搧火 | chuan2 feng1 shan1 huo3 | chuan2 feng1 you3 huo3 |
| 传神阿堵 | chuan2 shen2 a1 du3 | chuan2 shen2 e1 du3 |
| 床笫之私 | chuang2 zi3 zhi1 si1 | chuang2 di4 zhi1 si1 |
| 春华秋实 | chun1 hua1 qiu1 shi2 | chun1 hua2 qiu1 shi2 |
| 歠菽饮水 | chuo4 shu1 yin3 shui3 | pa2 shu1 yin3 shui3 |
| 大大落落 | da4 da luo1 luo1 | da4 da4 luo4 luo4 |
| 大雨滂沱 | da4 yu3 pang1 tuo2 | da4 yu3 pang2 tuo2 |
| 灯红酒绿 | deng1 hong2 jiu3 lu4 | deng1 hong2 jiu3 lü4 |
| 冬箑夏裘 | dong1 sha4 xia4 qiu2 | dong1 zha2 xia4 qiu2 |
| 洞见症结 | dong4 jian4 zheng1 jie2 | dong4 jian4 zheng4 jie2 |
| 斗筲穿窬 | dou3 shao1 chuan1 yu2 | dou4 shao1 chuan1 yu2 |
| 笃近举远 | du3 jin4 ju3 yuan3 | du3 jin4 ju3 juan3 |
| 断发纹身 | duan4 fa4 wen2 shen1 | duan4 fa1 wen2 shen1 |
| 额首称庆 | e2 shou3 cheng1 qing4 | e2 shou1 cheng1 qing4 |
| 耳濡目染 | er3 ru2 mu4 ran3 | er3 ru3 mu4 ran3 |
| 发怒冲冠 | fa4 nu4 chong1 guan1 | fa1 nu4 chong1 guan4 |
| 发上冲冠 | fa4 shang4 chong1 guan1 | fa1 shang4 chong1 guan4 |
| 发上指冠 | fa4 shang4 zhi3 guan1 | fa1 shang4 zhi3 guan4 |
| 反攻倒算 | fan3 gong1 dao4 suan4 | fan3 gong1 dao3 suan4 |
| 沸沸汤汤 | fei4 fei4 shang1 shang1 | fei4 fei4 tang1 tang1 |
| 纷红骇绿 | fen1 hong2 hai4 lu4 | fen1 hong2 hai4 lü4 |
| 粉白黛绿 | fen3 bai2 dai4 lu4 | fen3 bai2 dai4 lü4 |
| 粉骨捐躯 | fen3 gu3 juan1 qu1 | fen　gu　juan　qu3311 |
| 粉骨糜躯 | fen3 gu3 mi2 qu1 | fen　gu　mi　qu3321 |
| 粉面朱唇 | fen3 mian4 zhu1 chun2 | fen　mian　zhu　chun3412 |
| 粉身灰骨 | fen3 shen1 hui1 gu3 | fen　shen　hui　gu3113 |
| 风尘肮脏 | feng1 chen2 ang1 zang1 | feng chen ang zang |
| 风轻云淡 | feng1 qing1 yun2 dan4 | feng　qing　yun　dan1124 |
| 风姿绰约 | feng1 zi1 chuo4 yue1 | feng1 zi1 chuo1 yue2 |
| 冯河暴虎 | ping2 he2 bao4 hu3 | feng2 he2 bao4 hu3 |
| 负乘致寇 | fu4 sheng4 zhi4 kou4 | fu4 cheng2 zhi4 kou4 |
| 负债累累 | fu4 zhai4 lei3 lei3 | fu4 zhai lei4 lei4 |
| 高风劲节 | gao1 feng1 jing4 jie2 | gao1 feng1 jin4 jie2 |
| 葛屦履霜 | ge2 ju4 lü3 shuang1 | ge3 ju4 lü3 shuang1 |
| 各有所长 | ge4 you3 suo3 chang2 | ge4 you3 suo3 cheng2 |
| 攻城掠地 | gong1 cheng2 lüe4 di4 | gong1 cheng2 lüe3 di4 |
| 古肥今瘠 | gu3 fei2 jin1 ji2 | gu3 fei2 jin1 shou4 |
| 瓜葛相连 | gua1 ge2 xiang1 lian2 | gua1 ge3 xiang1 lian2 |
| 呱呱堕地 | gu1 gu1 duo4 di4 | gua1 gua1 duo4 di4 |
| 呱呱坠地 | gu1 gu1 zhui4 di4 | gua1 gua1 zhui4 di4 |
| 管窥蠡测 | guan3 kui1 li2 ce4 | guan3 kui1 li3 ce4 |
| 过都历块 | guo4 du1 li4 kuai4 | guo4 dou1 li4 kuai4 |
| 蒿目时艰 | hao1 mu4 shi2 jian1 | hang4 mu4 shi2 jian1 |
| 荷枪实弹 | he4 qiang1 shi2 dan4 | he2 qiang1 shi2 dan4 |
| 红男绿女 | hong2 nan2 lu4 nü3 | hong2 nan2 lü4 nü3 |
| 红情绿意 | hong2 qing2 lu4 yi4 | hong2 qing2 lü4 yi4 |
| 划粥割齑 | hua4 zhou1 ge1 ji1 | hua4 zhou1 ge1 jiu1 |
| 怀柔天下 | huai2 rou2 tian1 xia4 | huai rou tian xia |
| 回黄转绿 | hui2 huang2 zhuan3 lu4 | hui2 huang2 zhuan3 lü4 |
| 混水捞鱼 | hun2 shui3 lao1 yu2 | hun4 shui3 lao1 yu2 |
| 混水摸鱼 | hun2 shui3 mo1 yu2 | hun4 shui3 mo1 yu2 |
| 疾风劲草 | ji2 feng1 jing4 cao3 | ji2 feng1 jin4 cao3 |
| 鹡鸰在原 | ji2 ling2 zai4 yuan2 | xia4 ling2 zai4 yuan2 |
| 戟指怒目 | ji3 zhi3 nu3 mu4 | ji3 zhi3 nu3 zhang1 |
| 间不容发 | jian1 bu4 rong2 fa4 | jian4 bu4 rong2 fa4 |
| 间不容瞚 | jian1 bu4 rong2 shun4 | jian1 bu4 rong2 xi3 |
| 诘屈磝碻 | ji2 qu1 ao2 qiao1 | jie2 qu1 bing4 zhou4 |
| 诘屈聱牙 | ji2 qu1 ao2 ya2 | jie2 qu1 ao2 ya2 |
| 诘屈謷牙 | ji2 qu1 ao2 ya2 | jie2 qu1 da4 ya2 |
| 惊心动魄 | jing1 xin1 dong4 po4 | jing1 xing1 dong4 po4 |
| 九蒸三熯 | jiu3 zheng1 san1 han4 | jiu3 zheng1 san1 sheng1 |
| 酒绿灯红 | jiu3 lu4 deng1 hong2 | jiu3 lü4 deng1 hong2 |
| 君子好逑 | jun1 zi3 hao3 qiu2 | jun1 zi3 hao4 qiu2 |
| 扛鼎抃牛 | gang1 ding3 bian4 niu2 | kang2 ding3 bian4 niu2 |
| 咳唾成珠 | ke2 tuo4 cheng2 zhu1 | ke　tuo24 cheng2 zhu1 |
| 坑蒙拐骗 | keng1 meng1 guai3 pian4 | keng1 meng2 guai3 pian4 |
| 款曲周至 | kuan3 qu1 zhou1 zhi4 | kuan3 qu3 zhou1 zhi4 |
| 锒铛入狱 | lang2 dang1 ru4 yu4 | lang2 kang1 ru4 yu4 |
| 唠唠叨叨 | lao2 lao dao1 dao1 | lao1 lao1 dao1 dao1 |
| 梨花带雨 | li2 hua1 dai4 yu3 | li2 hu ai4 yu3 |
| 力有未逮 | li4 you3 wei4 dai4 | li4 you3 wei4 dai3 |
| 良贾深藏 | liang2 gu3 shen1 cang2 | liang2 jia3 shen1 cang2 |
| 陵劲淬砺 | ling2 jing4 cui4 li4 | ling2 jin4 cui4 li4 |
| 柳绿花红 | liu3 lu4 hua1 hong2 | liu3 lü4 hua1 hong2 |
| 柳绿桃红 | liu3 lu4 tao2 hong2 | liu3 lü4 tao2 hong2 |
| 露红烟绿 | lu4 hong2 yan1 lu4 | lu4 hong2 yan1 lü4 |
| 率尔操觚 | shuai4 er3 cao1 gu1 | shuai4 er2 cao1 gu1 |
| 绿暗红稀 | lu4 an4 hong2 xi1 | lü4 an4 hong2 xi1 |
| 绿鬓红颜 | lu4 bin4 hong2 yan2 | lü4 bin4 hong2 yan2 |
| 绿鬓朱颜 | lu4 bin4 zhu1 yan2 | lü4 bin4 zhu1 yan2 |
| 绿惨红愁 | lu4 can3 hong2 chou2 | lü4 can3 hong2 chou2 |
| 绿惨红销 | lu4 can3 hong2 xiao1 | lü4 can3 hong2 xiao1 |
| 绿肥红瘦 | lu4 fei2 hong2 shou4 | lü4 fei2 hong2 shou4 |
| 绿酒红灯 | lu4 jiu3 hong2 deng1 | lü4 jiu3 hong2 deng1 |
| 绿女红男 | lu4 nü3 hong2 nan2 | lü4 nü3 hong2 nan2 |
| 绿水青山 | lu4 shui3 qing1 shan1 | lü4 shui3 qing1 shan1 |
| 绿叶成阴 | lu4 ye4 cheng2 yin1 | lü4 ye4 cheng2 yin1 |
| 尨眉皓发 | manɡ2 mei2 hao4 fa4 | chou2 mei2 hao4 fa1 |
| 毛遂自荐 | mao2 sui4 zi4 jian4 | mao2 sui2 zi4 jian4 |
| 没金饮羽 | mo4 jin1 yin3 yu3 | mei2 jin1 yin3 yu3 |
| 没世无闻 | mo4 shi4 wu2 wen2 | mei2 shi4 wu2 wen2 |
| 面红面绿 | mian4 hong2 mian4 lu4 | mian4 hong2 mian4 lü4 |
| 默而识之 | mo4 er2 zhi4 zhi1 | mo4 er2 shi2 zhi1 |
| 谋无遗谞 | mou2 wu2 yi2 xu1 | mou2 wu2 yi2 er2 |
| 目瞪舌彊 | mu4 deng4 she2 qiang2 | mu4 deng4 she2 jiang4 |
| 内圣外王 | nei4 sheng4 wai4 wang2 | nei4 sheng4 wai4 zhu3 |
| 泥古拘方 | ni4 gu3 ju1 fang1 | ni　gu　ju　fang4311 |
| 泥名失实 | ni4 ming2 shi1 shi2 | ni　ming　shi　shi4212 |
| 逆行倒施 | ni4 xing2 dao4 shi1 | ni4 xing2 dao3 shi1 |
| 年高德卲 | nian2 gao1 de2 shao4 | nian2 gao1 de2 er2 |
| 宁缺毋滥 | ning4 que1 wu2 lan4 | ning4 que1 wu4 lan4 |
| 排忧解难 | pai2 you1 jie3 nan4 | pai2 you1 jie3 nan2 |
| 滂沱大雨 | pang1 tuo2 da4 yu3 | pang2 tuo2 da4 yu3 |
| 批亢捣虚 | pi1 kang4 dao3 xu1 | pi1 gang4 dao3 xu1 |
| 批亢抵巇 | pi1 gang1 di3 xi1 | pi　gang　di　xi1131 |
| 胼手胝足 | pian2 shou3 zhi1 zu2 | pian2 sho3 zhi1 zu2 |
| 帡天极地 | pinɡ2 tian1 ji2 di4 | ju2 tian1 ji2 di4 |
| 破璧毁珪 | po4 bi4 hui3 ɡui1 | po4 bi4 hui3 zhi3 |
| 破斧缺斨 | po4 fu3 que1 qiang1 | po4 fu3 que1 zhou1 |
| 弃书捐剑 | qi4 shu1 juan1 jian4 | qi　shu　juan　jian4114 |
| 砌红堆绿 | qi4 hong2 dui1 lu4 | qi4 hong2 dui1 lü4 |
| 牵强附会 | qian1 qiang3 fu4 hui4 | qian1 qiang2 fu4 hui4 |
| 强弓劲弩 | qiang2 gong1 jing4 nu3 | qiang2 gong1 jin4 nu3 |
| 俏成俏败 | xiao4 cheng2 xiao4 bai4 | qiao4 cheng2 qiao4 bai4 |
| 切身体会 | qie4 shen1 ti3 hui4 | qie1 shen1 ti3 hui4 |
| 擒奸擿伏 | qin2 jian1 ti1 fu2 | qin2 jian1 fa1 fu2 |
| 青山绿水 | qing1 shan1 lu4 shui3 | qing1 shan1 lü4 shui3 |
| 青枝绿叶 | qing1 zhi1 lu4 ye4 | qing1 zhi1 lü4 ye4 |
| 清风劲节 | qing1 feng1 jing4 jie2 | qing1 feng1 jin4 jie2 |
| 情不自禁 | qing2 bu4 zi4 jin1 | qing2 bu4 zi4 jin4 |
| 情长纸短 | qing2 chang2 zhi3 duan3 | qing　chang　zhi　duan2233 |
| 请君入瓮 | qing3 jun1 ru4 weng4 | qing3 jung1 ru4 weng4 |
| 穷形尽相 | qiong2 xing2 jin4 xiang4 | qiong2 xing2 ji4 xiang4 |
| 曲肱而枕 | qu1 gong1 er2 zhen3 | qu3 gong1 er2 zhen3 |
| 忍俊不禁 | ren3 jun4 bu4 jin1 | ren3 jun4 bu4 jin4 |
| 若即若离 | ruo4 ji2 ruo4 li2 | ruo4 ji4 ruo4 li2 |
| 三年五载 | san1 nian2 wu3 zai3 | san1 nian2 wu3 zai4 |
| 丧胆销魂 | sang4 dan3 xiao1 hun2 | sang4 hun2 xiao1 hun2 |
| 善善恶恶 | shan4 shan4 e4 e4 | shan4 shan4 wu4 e4 |
| 神魂荡飏 | shen2 hun2 dang4 yang2 | shen2 hun2 dang4 chen2 |
| 生杀予夺 | sheng1 sha1 yu3 duo2 | sheng1 sha1 yu4 duo2 |
| 鼪鼯之径 | sheng1 wu2 zhi1 jing4 | wei2 wu2 zhi1 jing4 |
| 鼪鼬之迳 | sheng1 you4 zhi1 jing4 | tian1 you4 zhi1 jing4 |
| 施绯拖绿 | shi1 fei1 tuo1 lu4 | shi1 fei1 tuo1 lü4 |
| 视丹如绿 | shi4 dan1 ru2 lu4 | shi4 dan1 ru2 lü4 |
| 瘦骨嶙峋 | shou4 gu3 lin2 xun2 | shou4 gu3 li2 xun2 |
| 书不尽言 | shu1 bu4 jin4 yan2 | shu　bu　jin　yan1442 |
| 书声琅琅 | shu1 sheng1 lang2 lang2 | shu1 sheng1 lang3 lang3 |
| 霜凋夏绿 | shuang1 diao1 xia4 lu4 | shuang1 diao1 xia4 lü4 |
| 水长船高 | shui3 zhang3 chuan2 gao1 | shui　zhang　chuan　gao3321 |
| 顺蔓摸瓜 | shun4 wan4 mo1 gua1 | shun4 man4 mo1 gua1 |
| 说白道绿 | shuo1 bai2 dao4 lu4 | shuo1 bai2 dao4 lü4 |
| 薮中荆曲 | sou3 zhong1 jing1 qu3 | sou3 zhong1 ji2 qu3 |
| 泰山磐石 | tai shan1 pan2 shi2 | tai4 shan1 pan2 shi2 |
| 桃红柳绿 | tao2 hong2 liu3 lu4 | tao2 hong2 liu3 lü4 |
| 靦颜人世 | mian3 yan2 ren2 shi4 | tian3 yan2 ren2 shi4 |
| 同室操戈 | tong2 shi4 cao1 ge1 | tong2 shi4 sao1 ge1 |
| 同文共轨 | tong2 wen2 gong4 gui3 | tong　wen　gong　gui2243 |
| 脱白挂绿 | tuo1 bai2 gua4 lu4 | tuo1 bai2 gua4 lü4 |
| 玩岁愒月 | wan2 sui4 kai4 yue4 | wan2 sui4 yi1 yue4 |
| 汪洋自恣 | wang1 yang2 zi4 zi4 | wang1 yang2 zi4 zi1 |
| 唯唯诺诺 | wei2 wei2 nuo4 nuo4 | wei3 wei3 nuo4 nuo4 |
| 委曲求全 | wei3 qu1 qiu2 quan2 | wei3 qu3 qiu2 quan2 |
| 味同嚼蜡 | wei4 tong2 jiao2 la4 | wei4 tong2 jiao2 cu4 |
| 握发吐哺 | wo4 fa4 tu3 bu3 | wo4 fa1 tu3 bu3 |
| 握发吐飧 | wo4 fa4 tu3 sun1 | wo4 fa1 tu3 sun1 |
| 物阜民安 | wu4 fu4 min2 an1 | wu4 fu3 min2 an1 |
| 物竞天择 | wu4 jing4 tian1 ze2 | wu4 jin4 tian1 ze2 |
| 物美价廉 | wu4 mei3 jia4 lian2 | jia4 lian2 wu4 mei3 |
| 瑕瑜互见 | xia2 yu2 hu4 jian4 | xia2 yu2 hu4 xian4 |
| 咸阳一炬 | xian2 yang2 yi1 ju4 | xian2 yang2 yi1 ju3 |
| 挦毛捣鬓 | xian2 mao2 dao3 bin4 | tun2 mao2 dao3 bin4 |
| 挦绵扯絮 | xian2 mian2 che3 xu4 | chan2 mian2 che3 xu4 |
| 挦章撦句 | xian2 zhang1 zong1 ju4 | long2 zhang1 zong1 ju4 |
| 详情度理 | xiang2 qing2 duo2 li3 | xiang2 qing2 du4 li3 |
| 橡茹藿歠 | xiang4 ru2 huo4 chuo4 | xiang　ru　huo　chuo4244 |
| 枵腹终朝 | xiao1 fu4 zhong1 zhao1 | xiao1 fu4 zhong1 chao2 |
| 鸮鸣鼠暴 | xiao1 ming2 shu3 bao4 | zhang1 ming2 shu3 bao4 |
| 鸮鸟生翼 | xiao1 niao3 sheng1 yi4 | qing1 niao3 sheng1 yi4 |
| 鸮啼鬼啸 | xiao1 ti2 gui3 xiao4 | niao3 ti2 gui3 xiao4 |
| 鸮心鹂舌 | xiao1 xin1 li2 she2 | ren2 xin1 li2 she2 |
| 蝎蝎螫螫 | xie1 xie1 zhe2 zhe2 | xie1 xie1 zhe1 zhe1 |
| 挟势弄权 | xie2 shi4 nong4 quan2 | jia1 shi4 nong4 quan2 |
| 心细如发 | xin1 xi4 ru2 fa4 | xin1 xi4 ru2 fa1 |
| 休明盛世 | xiu1 ming2 sheng4 shi4 | xiu　ming　sheng　shi1244 |
| 修旧利废 | xiu1 jiu4 li4 fei4 | xiu　jiu　li　fei1444 |
| 朽骨重肉 | xiu3 gu3 chong2 rou4 | xiu3 gu3 zhong4 rou4 |
| 悬车之年 | xuan2 che1 zhi1 nian2 | xuan　che　zhi　nian2112 |
| 悬龟系鱼 | xuan2 guiji14 yu2 | xuan2 gui@ji14 yu2 |
| 悬崖绝壁 | xuan2 ya2 jue2 bi4 | xuan　ya　jue　bi2224 |
| 一朝千里 | yi1 zhao1 qian1 li3 | yi　zhao　qian　li1113 |
| 一朝之患 | yi1 zhao1 zhi1 huan4 | yi　zhao　zhi　huan1114 |
| 一哄而起 | yi1 hong4 er2 qi3 | yi1 hong1 er2 qi3 |
| 一哄而散 | yi1 honɡ4 er2 san4 | yi1 hong1 er2 san4 |
| 一哄而上 | yi4 hong1 er2 shang4 | yi1 hong3 er2 shang4 |
| 一模一样 | yi1 mu2 yi1 yang4 | yi1 mo2 yi1 yang4 |
| 一丘之貉 | yi1 qiu1 zhi1 he2 | yi1 qiu1 zhi1 he4 |
| 一邱之貉 | yi1 qiu1 zhi1 he2 | yi1 qiu1 zhi1 he4 |
| 一日之长 | yi1 ri4 zhi1 chang2 | yi1 ri4 zhi1 zhang3 |
| 移宫换羽 | yi2 gong1 huan4 yu3 | yi2 dong1 huan4 yu3 |
| 以噎废飡 | yi3 ye1 fei4 can1 | yi3 ye1 fei4 guang1 |
| 喑噁叱咤 | yin1 e4 chi4 zha4 | yin1 wu4 chi4 zha4 |
| 淫言媟语 | yin2 yan2 xie4 yu3 | yin2 yan2 liang3 yu3 |
| 引吭高声 | yin3 hang2 gao1 sheng1 | yin　hang　gao　sheng3211 |
| 永永无穷 | yong3 yong3 wu2 qiong2 | yong3 shi4 wu2 qiong2 |
| 用行舍藏 | yong4 xing2 she3 cang2 | yong4 xing2 cang2 she3 |
| 有的放矢 | you3 di4 fang4 shi3 | you3 di3 fang4 shi3 |
| 杅穿皮蠹 | yu2 chuan1 pi2 du4 | yu2 chuan1 shui3 du4 |
| 约定俗成 | yue1 ding4 su2 cheng2 | yue4 ding4 su2 cheng2 |
| 泽被后世 | ze2 pi1 hou4 shi4 | ze2 bei4 hou4 shi4 |
| 乍暖还寒 | zha4 nuan3 huan2 han2 | zha4 nuan3 hai2 han2 |
| 蒸沙为饭 | zheng1 sha1 wei2 fan4 | zheng　sha　wei　fan1124 |
| 指囷相赠 | zhi3 qun1 xiang1 zeng4 | zhi3 que4 xiang1 zeng4 |
| 质而不野 | zhi4 er2 bu4 ye3 | zhi　er　bu　ye4243 |
| 重厚寡言 | zhong4 hou4 gua3 yan2 | zhong　hou　gua　yan4432 |
| 朱颜鹤发 | zhu1 yan2 he4 fa4 | zhu1 yan2 he4 fa1 |
| 朱颜绿发 | zhu1 yan2 lü4 fa4 | zhu1 yan2 lü4 fa1 |
| 抓耳搔腮 | zhua1 er3 sao1 sai1 | zhua?er13 sao1 sai1 |
| 装模作样 | zhuang1 mu2 zuo4 yang4 | zhuang1 mo2 zuo4 yang4 |
| 壮士解腕 | zhuang4 shi4 jie3 wan4 | zhuang4 shi　jie　wan434 |
| 足尺加二 | zu2 chi3 jia1 er4 | zu2 chi3 ji?er4 |
| 作舍道边 | zuo4 she4 dao4 bian1 | zuo4 she3 dao4 bian1 |
