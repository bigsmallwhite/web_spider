## 分析：
1、采用selenium驱动浏览器，xpath，re等解析页面，csv格式保存

2、分析每页不实信息url，发现只需在'https://service.account.weibo.com/index?type=5&status=0&page='末尾更改数字即可获取不同页码的具体微博信息

3、由于尽可能的多获取特征，故需要点击每条信息的原文

## 流程：
1、登录微博，到不实信息页面

2、根据爬取的数据量，设置爬取页码

3、对每一页的信息链接进行遍历，获取每条微博的信息特征

4、保存每一条信息到csv文件

