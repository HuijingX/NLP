# NLP Projects

## Text Classification

### 头条新闻分类
根据头条新闻标题自动分类
数据样例：

| label | label_desc | sentence|keywords|
| --- | --- | --- | --- |
| 108 |  news_edu| 上课时学生手机响个不停，老师一怒之下把手机摔了，家长拿发票让老师赔，大家怎么看待这种事||
| 104 |  news_finance| 商赢环球股份有限公司关于延期回复上海证券交易所对公司2017年年度报告的事后审核问询函的公告| 商赢环球股份有限公司,年度报告,商赢环球,赢环球股份有限公司,事后审核问询函,上海证券交易所|


* [使用TFIDF构建baseline模型](https://github.com/HuijingX/NLP/blob/main/%E5%A4%B4%E6%9D%A1%E6%96%B0%E9%97%BB%E5%88%86%E7%B1%BB_%E6%95%B0%E6%8D%AE%E5%88%86%E6%9E%90%26%E6%9E%84%E5%BB%BAbaseline.ipynb)
* [使用TextCNN+新浪词向量构建模型](https://github.com/HuijingX/NLP/blob/main/%E5%A4%B4%E6%9D%A1%E6%96%B0%E9%97%BB%E5%88%86%E7%B1%BB_TextCNN.ipynb)
* [使用BERT构建模型](https://github.com/HuijingX/NLP/blob/main/%E5%A4%B4%E6%9D%A1%E6%96%B0%E9%97%BB%E5%88%86%E7%B1%BB_BERT.ipynb)
* [使用BERT+Head构建模型](https://github.com/HuijingX/NLP/blob/main/%E5%A4%B4%E6%9D%A1%E6%96%B0%E9%97%BB%E5%88%86%E7%B1%BB_BERT%2BHead.ipynb)

## Text Similarity

### 蚂蚁金融语义相似度分析
根据蚂蚁金融数据自动判定该对句子语义相似与否
数据样例：
| sentence1 | sentence2 | label |
| --- | --- | --- |
| 支付宝系统点我的里面没有花呗这一项 | 我下载支付宝怎么没有花呗的 | 1 |
| 蚂蚁借呗等额还款可以换成先息后本吗 | 借呗有先息到期还本吗 | 0 |

* [使用ESIM构建模型](https://github.com/HuijingX/NLP/blob/main/%E8%9A%82%E8%9A%81%E9%87%91%E8%9E%8D%E8%AF%AD%E4%B9%89%E7%9B%B8%E4%BC%BC%E5%BA%A6_ESIM.ipynb)
* [使用BERT+对抗训练构建模型](https://github.com/HuijingX/NLP/blob/main/%E8%9A%82%E8%9A%81%E9%87%91%E8%9E%8D%E8%AF%AD%E4%B9%89%E7%9B%B8%E4%BC%BC%E5%BA%A6_BERT%2B%E5%AF%B9%E6%8A%97%E8%AE%AD%E7%BB%83.ipynb)
* [使用BERT+UDA数据增强构建模型](https://github.com/HuijingX/NLP/blob/main/%E8%9A%82%E8%9A%81%E9%87%91%E8%9E%8D%E8%AF%AD%E4%B9%89%E7%9B%B8%E4%BC%BC%E5%BA%A6_BERT%2BUDA.ipynb)

## Text Summarization

### NLPCC2017
根据文本进行自动摘要
数据样例：
| title | content |
| --- | --- |
| 知情人透露章子怡怀孕后,父母很高兴。章母已开始悉心照料。据悉,预产期大概是12月底 | 四海网讯,近日,有媒体报道称:章子怡真怀孕了!报道还援引知情人士消息称,“章子怡怀孕大概四五个月,预产期是年底前后,现在已经不接工作了。”这到底是怎么回事?消息是真是假?针对此消息,23日晚8时30分,华西都市报记者迅速联系上了与章子怡家里关系极好的知情人士,这位人士向华西都市报记者证实说:“子怡这次确实怀孕了。她已经36岁了,也该怀孕了。章子怡怀上汪峰的孩子后,子怡的父母亲十分高兴。子怡的母亲,已开始悉心照料女儿了。子怡的预产期大概是今年12月底。”当晚9时,华西都市报记者为了求证章子怡怀孕消息,又电话联系章子怡的亲哥哥章子男,但电话通了,一直没有人接听。有关章子怡怀孕的新闻自从2013年9月份章子怡和汪峰恋情以来,就被传N遍了!不过,时间跨入2015年,事情却发生着微妙的变化。2015年3月21日,章子怡担任制片人的电影《从天儿降》开机,在开机发布会上几张合影,让网友又燃起了好奇心:“章子怡真的怀孕了吗?”但后据证实,章子怡的“大肚照”只是影片宣传的噱头。过了四个月的7月22日,《太平轮》新一轮宣传,章子怡又被发现状态不佳,不时深呼吸,不自觉想捂住肚子,又觉得不妥。然后在8月的一天,章子怡和朋友吃饭,在酒店门口被风行工作室拍到了,疑似有孕在身!今年7月11日,汪峰本来在上海要举行演唱会,后来因为台风“灿鸿”取消了。而消息人士称,汪峰原来打算在演唱会上当着章子怡的面宣布重大消息,而且章子怡已经赴上海准备参加演唱会了,怎知遇到台风,只好延期,相信9月26日的演唱会应该还会有惊喜大白天下吧。 |
| 青海首次野外发现濒危大火烈鸟 尚不清楚具体来源 | 中新社西宁11月22日电(赵凛松)青海省林业厅野生动植物和自然保护区管理局高级工程师张毓22日向中新社记者确认:“经过中国林业科学院、中科院新疆生态与地理研究所和青海省林业厅的共同认定,出现在青海省海西州境内的三只体型较大的鸟为世界极度濒危的红鹳目红鹳科红鹳属的大红鹳。”11月18日,青海省海西州可鲁克湖—托素湖国家级陆生野生动物疫源疫病监测站在野外监测巡护过程中,在可鲁克湖西南岸入水口盐沼滩发现三只体型较大的鸟类。张毓说:“此前在该区域从未发现过这种体型的鸟类。”可鲁克湖—托素湖位于青海省柴达木盆地东北部,海拔2800米,水域湿地环境内的优势种动物主要是水禽,共有30余种。根据拍摄的照片以及视频,张毓根据动物学体型得出了初步结论,然后会同中国林业科学院和中科院新疆生态与地理研究所的相关专家,确认了这三只鸟为红鹳目红鹳科红鹳属的大红鹳。大红鹳也称为大火烈鸟、红鹤等,三只鸟类特征为大红鹳亚成体。根据世界自然保护联盟、世界濒危动物红色名录,该鸟主要分布于非洲、中亚、南亚等区域,分布广、种群数量较大,无威胁因子,以往在中国并无分布。但1997年在新疆野外首次发现并确定该鸟在中国境内有分布,为中国鸟类新纪录,2012年在四川也发现一只该鸟亚成体。此次野外发现在中国属第三次。“我们现在还无法判断这三只鸟从何而来。不过我个人倾向于是从中亚国家迁徙至此。”张毓强调说,该种鸟国内也有人工饲养,因此也有人判断为从动物园逃逸。“我们对这三只鸟进行了详尽的记录,如果明年这个时间还在此地出现这种鸟,那就能肯定是迁徙的鸟类,而不是从动物园里跑出来的。”由于目前可鲁克湖—托素湖已开始结冰,鸟类采食困难,不排除三只鸟由于无法获得能量补给而进行远距离迁飞的可能。青海省林业厅野生动物行政主管部门将随时做好野外救护的各项准备工作。 |

* [使用Seq2Seq构建模型](https://github.com/HuijingX/NLP/blob/main/%E6%96%87%E6%9C%AC%E6%91%98%E8%A6%81_Seq2Seq.ipynb)
* [使用BERT构建模型](https://github.com/HuijingX/NLP/blob/main/%E6%96%87%E6%9C%AC%E6%91%98%E8%A6%81_BERT.ipynb)
 
