# Aazhen-V3.0
自研JavaFX图形化漏洞扫描工具，支持ThinkPHP 2.x RCE，Thinkphp5 5.0.22/5.1.29RCE，ThinkPHP5 5.0.23RCE和ThinkPHP5 SQL注入漏洞和敏感信息泄露漏洞的漏洞检测，以及命令执行的功能。漏洞POC基本适用ThinkPHP全版本漏洞。

很多小伙伴和我反馈Java版本不兼容的问题，由于是java,版本问题这确实没办法彻底解决，除非用每个版本开发一遍，但太耗时耗力，所以这次也是换成了更加普遍的jdk-1.8版本，也就是java8同时，也有小伙伴反馈java swing太老，所以这次也用JavaFX重构了整个框架，让界面更加清新-干净-高效。最后，也采纳了一些比较懒的朋友的建议，把jar包换成了exe，这样就不用命令运行，直接双击搞定。日后有更好的建议欢迎大家在Issues上面提，也可以来我的博客私信我，博客地址在简介里，欢迎交流技术以及工具的反馈。

因为刚学java没多久，所以工具做得不是很好，功能不多，非常简陋，会一直更新持续改进，用java拯救太阳系！
## 2022年4月25日->Aazhen-V3.0
**功能**：

1、支持ThinkPHP 2.x RCE，Thinkphp5 5.0.22/5.1.29RCE，ThinkPHP5 5.0.23RCE和ThinkPHP5 SQL注入漏洞和敏感信息泄露漏洞的漏洞检测。

2、上述漏洞中除了信息泄露以外的所有RCE漏洞支持命令执行功能。

3、一键检测所有漏洞。

**工具简介与界面展示**:

1、用JavaFX重构整个框架，完全代替了之前的Java Swing。
2、页面干净整洁，没用的组件通通不要。
3、工具从原来的ThinkphpScannerGUI正式改名为Aazhen。每个男人的心中都有一个属于他的阿珍，这个工具也是我的处女作，工具很落后，没什么人用，完全个人爱好，所以不好的地方轻点喷。

<img src="https://user-images.githubusercontent.com/64825932/165022740-0d3aab02-7da3-4921-8c0f-f38dedd5c775.png" width="400px">



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


