# 2023年3月24日RexHa（Aazhen）-V 1.0
取消了其他java版本，只留java8/jdk1.8版本的。同时修改了部分源码，优化poc，运行方式有变动，启动方式为：

java -javaagent:rexha.jar -jar rexha.jar


<img src="https://user-images.githubusercontent.com/64825932/227475593-e2422e32-8ccb-4e84-a6bb-30fec3dd8c4a.png" width="400px">




# 2022年10月23日RexHa（Aazhen）-V 1.0

很多小伙伴反馈说java18那个版本无法运行，所以我又新增了一个jdk1.8版本的，这次绝壁没问题了。jdk1.8非常稳定，建议大家还是下载jdk1.8的版本。后续会陆续添加jdk11和14版本的，无奈，java开发东西就是得考虑到版本问题。望谅解。

# RexHa（Aazhen）新版本！！ -V 1.0
hello，好久没更，工具改名成RexHa。工具的教程在我博客上（很详细）：
https://blog.csdn.net/weixin_43847838/article/details/127396997?spm=1001.2014.3001.5501
最新版RexHa工具的功能以及特点：
我是用java18开发的，jdk版本太低的话可能会运行不起来。

①HttpClient替代旧版HttpUrlConection

②多线程并发

③重写了 7 个Payload

上一个版本中，支持检测的漏洞只有4个，这次我直接加到了7个，基本上覆盖了ThinkPHP的大部分版本，支持扫描的漏洞分别是：
    ThinkPHP-2.x-RCE，
    ThinkPHP-5.0.23-RCE，
    ThinkPHP5.0.x-5.0.23通杀RCE，
    ThinkPHP5-SQL注入&敏感信息泄露，
    ThinkPHP 3.x 日志泄露NO.1，
    ThinkPHP 3.x 日志泄露NO.2，
    ThinkPHP 5.x 数据库信息泄露。
而且每一种漏洞都是经过靶场+实战验证，每个Payload我都能保证不会有问题，而且能够精准判断。

④取消了旧版的命令执行功能

⑤Aazhen改名成RexHa

谢谢我的猫~❤️ 工具多了很多猫咪的元素在里面，本文后面也会细说。

⑥url输入格式判断

新版本的界面展示如下:

<img src="https://user-images.githubusercontent.com/64825932/196480082-2fd8cb5a-eb20-4743-a893-5de22b89e8cf.png" width="400px">

# Aazhen-V3.1 jar版本免费开源
因为很多小伙伴说exe只支持win，linux或其他系统不兼容等问题，所以我今天把这个工具开源了，打包成了jar包可以下载，代码写得很烂，毕竟专业不是编程的，水平不够，见谅。


# Aazhen-V3.1
自研JavaFX图形化漏洞扫描工具，支持ThinkPHP 2.x RCE，Thinkphp5 5.0.22/5.1.29RCE，ThinkPHP5 5.0.23RCE和ThinkPHP5 SQL注入漏洞和敏感信息泄露漏洞的漏洞检测，以及命令执行的功能。漏洞POC基本适用ThinkPHP全版本漏洞。

很多小伙伴和我反馈Java版本不兼容的问题，由于是java,版本问题这确实没办法彻底解决，除非用每个版本开发一遍，但太耗时耗力，所以这次也是换成了更加普遍的jdk-1.8版本，也就是java8。同时，也有小伙伴反馈java swing太老，所以这次也**用JavaFX重构了整个框架**，让界面更加清新-干净-高效。最后，也采纳了一些比较懒的朋友的建议，**把jar包换成了exe**，这样就不用命令运行，**直接双击搞定**。日后有更好的建议欢迎大家在Issues上面提，也可以来我的博客私信我，**博客地址在简介里**，欢迎交流技术以及工具的反馈。

因为刚学java没多久，所以工具做得不是很好，功能不多，非常简陋，会一直更新持续改进，用java拯救太阳系！

## 2022年4月25日->Aazhen-V3.1
3.0刚发布一个小时就有小伙伴跟我反馈工具有bug，bug为“ThinkPHP5 SQL注入漏洞和敏感信息泄露漏洞”漏洞检测功能的输出问题，逻辑判断有点小问题，后面经过vulhub和fofa靶场的测试，bug已经修复，输出能够正常显示。这里要感谢细心的![@kaaxcn](https://github.com/kkaaxcn)，让我及时发现问题。

下面是修复后的输出，恢复正常显示：

<img src="https://user-images.githubusercontent.com/64825932/165042278-8c719411-6989-4130-81e9-e02283660de3.png" width="400px">




## 2022年4月25日->Aazhen-V3.0
**功能**：

1、支持ThinkPHP 2.x RCE，Thinkphp5 5.0.22/5.1.29RCE，ThinkPHP5 5.0.23RCE和ThinkPHP5 SQL注入漏洞和敏感信息泄露漏洞的漏洞检测。

2、上述漏洞中除了信息泄露以外的所有RCE漏洞支持命令执行功能。

3、一键检测所有漏洞。

**工具简介**:

1、用JavaFX重构整个框架，完全代替了之前的Java Swing。
2、页面干净整洁，没用的组件通通不要。
3、工具从原来的ThinkphpScannerGUI正式改名为Aazhen。每个男人的心中都有一个属于他的阿珍，这个工具也是我的处女作，工具很落后，没什么人用，完全个人爱好，所以不好的地方轻点喷。

<img src="https://user-images.githubusercontent.com/64825932/165022740-0d3aab02-7da3-4921-8c0f-f38dedd5c775.png" width="400px">

**界面展示**：

1、外观

<img src="https://user-images.githubusercontent.com/64825932/165023241-5d358a78-ea30-4435-b63a-93480ea220f1.png" width="500px">

①界面半透明 ②有了工具的小logo ③鼠标是一个小太阳 ④用了三种布局方式组合在一起。

2、漏洞检测演示

一键检测展示：

<img src="https://user-images.githubusercontent.com/64825932/165024107-186484d9-ad8d-49d6-855e-e53025d728cf.png" width="500px">

3、命令执行模块演示
选择刚刚检测出来的漏洞版本，然后才能命令执行，输出结果：

<img src="https://user-images.githubusercontent.com/64825932/165024541-3a49cf8d-462c-4012-a8e5-c8be16fabbec.png" width="500px">

<img src="https://user-images.githubusercontent.com/64825932/165024860-fb180c14-cb55-4073-8761-af09d8ab590b.png" width="500px">


4、菜单栏就不做展示了，大家可以自己下载来玩玩。







## 2022年3月17日->工具ThinkphpScannerGUI-V1.0更新为V2.0版本。
**新增功能**：1、文件导入 2、批量检测

**优化**：重新设计了语句的输出，让输出不再那么“眼花缭乱”。

<img src="https://user-images.githubusercontent.com/64825932/158748973-ddeba0c5-ccbb-4fb8-9443-fa55caf86ab4.png" width="500px">

2.0版的扫描，以vulhub docker靶场为例：

<img src="https://user-images.githubusercontent.com/64825932/158749248-984614e4-a75d-4aa0-ac53-f4b9498c24f4.png" width="500px">

## 2022年2月28日->工具ThinkphpScannerGUI-V1.0发布
**功能**：支持单目标ip的扫描

<img src="https://user-images.githubusercontent.com/64825932/155970803-c7bdc45c-f1ea-4ca3-b329-098a1c907969.png" width="500px">
1.工具使用步骤：

下载jar包之后，命令行输入 java -jar JAVA_ThinkphpScannerGUI_Done.jar即可运行。
2.支持检测的漏洞

<img src="https://user-images.githubusercontent.com/64825932/155971045-08adae08-bd97-41e2-afc8-e0d0ef41c424.png" width="500px">


