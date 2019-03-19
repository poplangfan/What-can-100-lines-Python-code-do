# Python100
100行以内的Pyhton代码可以做哪些有意思的事<br>
觉得有意思就尝试了下，希望大家可以补充<br>
## 关于运行环境的补充
Python3.6<br>
Pycharm2017.2.3<br>
关于用到的Python库,有些是自带的，有些需要安装，但是都很简单，用过Python的人都应该知道，不再赘述<br>

## 关于代码的简单介绍
- lol.py 运行该文件可直接获取所有英雄皮肤。<br>
- wechat_auto_recovery.py 运行此文件需借助itchat库，运行后扫码登录，可实现好友来信息通知到文件助手，并回复他自定义好的内容<br>
- wechat_friends_info.py 运行此文件需借助itchat库，运行后扫码登录,可实现好友信息统计（性别，昵称，所在城市，个性签名，视自己需要而定），并保存到csv文件。<br>
- tieba.py 此文件只可以实现简单的发帖，循环发固定内容，进阶版会连接MongoDB数据库，实现网络信息的获取，不重复，随机发。
- tieba 文件夹是tieba.py的进阶版，在这个版本里，主要做了以下改进
  - 为了实现消息的充足性，用get_info从网上获取信息，并保存到MongoDB数据库；
  - 为了实现发帖的随机性，用random随机函数；
  - 为了保证意外情况造成的程序终止，获取信息和发帖均实现了和数据库的同步，确保不做无用功。
- wordCloud 文件夹是用jiebe库进行分词，并用wordcloud库进行词云展示的项目，代码仅有16行，展示的是2019政府工作报告，内附政府工作报告文件。 