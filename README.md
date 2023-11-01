# 微博评论情感二分类
基于bert的中文微博评论情感二分类,predict的输出结果为[-0.5,0.5]之间的一个数值，数值约高表示positive的可能性越大，数值越低表示negative的可能性越大。
如果想直接输出分类结果，直接把predict中argmax后的判断语句去除即可，1表示positive的可能性，0表示negtive的可能性。
