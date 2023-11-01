# bert_weibo_sentiment_analysis
基于bert的中文微博评论情感二分类。

预训练模型使用chenese-bert-wwm-ext，在项目所在目录下新建名称为chenese-bert-wwm-ext的目录存放huggingface下载来的预训练模型。
在项目所在目录下，新建名称为model的目录，运行main.py微调，模型保存在model目录下。
在config.py中修改载入模型的路径，运行inference.py即可进行推理。inference.py的输出结果为[-0.5,0.5]之间的一个数值，数值约高表示positive的可能性越大，数值越低表示negative的可能性越大。 如果想直接输出分类结果，直接把inference.py的predict中argmax后的判断语句去除即可，argmax的结果1表示positive的可能性，0表示negtive的可能性。
