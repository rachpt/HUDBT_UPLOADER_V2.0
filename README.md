版权归属：华科蝴蝶

测试环境：win10 + python3.6.4  + qbit4.1.5

支持的站点： 
+ 教育网：北邮人、北洋园、南洋、蒲公英、麦田、葡萄
+ 公网：TTG、HDChina、MTeam、天空、HDHome、朋友、OurBits


更新记录：copy自HUDBT：<https://hudbt.hust.edu.cn/details.php?id=142028&hit=1> 

2019-06-12：自反馈
修复北邮人RSS模式，[color=Red]RSS刷新设置时间为0表示全部接受，刷新时间回归默认的10分钟。解释说明：0表示接受RSS订阅里的所有任务加入qbt, 每10分钟刷新一次啊链接；其他数字，以5为例，每5分钟刷新一次啊，接受订阅里过去5分钟发布的种子加入qbt。建议：0作为一次性的，另外的是长时间的（默认10分钟）。

2019-06-12：[MatthewLXJ](https://hudbt.hust.edu.cn/userdetails.php?id=124176)反馈  
修复未完成关闭备份后重新打开任务添加错误；修复南洋RSS获取链接爬取HTML网页失败错误。

2019-06-12：[rach](https://hudbt.hust.edu.cn/userdetails.php?id=107055)反馈  
增加标题两边去空格处理，撒魔力3000。

2019-06-13：发现经常传不了图片链接上来。但是根据imdb等生成的简介又可以，待解决。——>已修复。
ut转qbit，1000多种子，休息几天。

2019-06-13：增加种子判断，30天期限删除（可以在客户端设置标签为“保留”则跳过删除）。

2019-06-14：基本上修复图片链接获取失败的bug，还剩下解析出简介中的mediainfo使其规范化（本身可以自己生成，但是有的站点自己制作的mediainfo带有制作者信息，为了表示感谢还是尽量遵循原作）

2019-06-14: 北洋园RSS获取不到图片。待修复——>已修复。

2019-06-15：mediainfo方案基本成型，待测试。——>BYR补齐，完成测试。

2019-06-16：需要增加iPad这个分类的判断，待修。——>已增加。

2019-06-16：馒头有的图片不能正常显示，地址需要unquote，待修复。——>已修复。

2019-06-17：订阅漏掉部分？刷新耗时，需要更改规则检验确定时间间隔。——>已修复。

2019-06-17：ut转qbt，折腾，欲增加reseed功能，测试中……（蝴蝶的搜索精度太惨了）

![](https://s2.ax1x.com/2019/06/17/VbJoRg.png)

![](https://s2.ax1x.com/2019/06/23/ZPWwlj.png)

2019-06-18：设置skip_checking，重做种跳过hash检验，直接辅种。上边第一个图没有跳过验证所以会显示检查中。

2019-06-22：集成reseed功能，测试中……几天下来1000+种子还是挺给力的。具体步骤参考蝴蝶原种子链接。

2019-06-23：部分种子下载完发布失败，已修复。发布之后立即删除缓存种子。

2019-06-25：frds出现了checking your browser before accessing ... anti robot 策略。还没想好怎么解决，暂不支持了~

2019-07-04：添加支持hdhome，测试中…… 

2019-07-05：添加支持麦田，测试中……

2019-07-08：[rach](https://hudbt.hust.edu.cn/userdetails.php?id=107055)反馈  ，修改手动上传bug一枚。

2019-07-09：再次添加CMCT，感动……

