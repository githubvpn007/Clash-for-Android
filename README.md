# Clash-for-Android
Clash，Clash教程，Clash配置，Clash使用教程，Clash安卓版本  

  
简介
----

Clash 是一个使用 Go 语言编写，基于规则的跨平台代理软件核心程序。  
Clash for Android 是安卓系统上的一款 Clash 客户端。  
支持的协议：Vmess, Shadowsocks, Snell, SOCKS5, ShadowsocksR[2.1.1版本开始支持]  

**特点：**  
- 可随时切换代理模式及节点
- 支持节点批量延迟测试
- 通过托管链接一键配置
- 规则命中分析
- 日志输出  


准备
----
1.准备Android 系统 5.0+ 以上的手机  
[2.下载安装](https://github.com/Kr328/ClashForAndroid/releases)  
3.准备订阅代理服务器，  如果你还没有订阅代理服务器 [请看完这里](https://github.com/githubvpn007/v2rayNvpn)   



<br/>


开始教程
----

**首先我们需要知道：Clash for Android 支持两种导入配置文档的方式 **  

1.URL （订阅）  
2.本地导入

<br/>

## 一。URL （订阅）  


(1) 请先登陆机场官网，进入“界面”页面，复制 Clash 订阅地址, 如果你不知道如何获取订阅地址 [请看这里](https://github.com/githubvpn007/v2rayNvpn#%E8%8A%82%E7%82%B9%E5%88%86%E4%BA%AB)  



(2)复制好了Clash订阅之后打开Clash for Android应用程序。请点击**配置**  

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/1.jpg) 

(3)新弹出的窗口中点击**新配置** .然后选择从URL导入。在对应地方填写**订阅地址**并保存。


![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/2.jpg) 


(4)选中 我们刚刚配置的订阅，表示我们将使用这个订阅的代理服务器联网  

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/3.jpg)   


(5)回到首页 点击开关，即可进行代理。会提示是否同意创建VPN，请点击**允许**。

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/4.jpg)  

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/5.jpg)  



(6)如果你想切换代理服务器等操作 可以在开启代理后，可以点击中间的代理选项卡，进入策略组面板，在这里可以切换节点。直接点击你想要的节点即可进行切换。

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/6.jpg)  


(7)在 "国外流量" 选项卡下显示的节点就是此订阅连接的所有节点，其中 **直接连接** 是默认存在的， 选中它的话就表示 你手机的所有请求不走代理服务器

(6)点击⚡图标可以进行延迟测试，测试结果将显示在节点名称右侧。 



<br/>
<br/>

## 二。本地文件导入  

点击 **配置** 👉 **新配置** 👉 **从文件导入**，然后从本地文件夹选择自己要导入的配置文档。
某些厂商的ROM可能报如下错误，请选择其他文件管理器导入

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/7.png)


<br/>
<br/>


## 三。查询日志

点击**日志**面板，然后选择**Clash日志捕捉工具**即可抓取日志。默认是关闭日志的，以防内存溢出。
 
![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/8.jpg) 
![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/9.jpg) 


## 四。分应用代理  

点击**设置** 👉 **网络**，最下方可以设置**分应用代理**。  
点击**访问控制模式**可以切换黑白名单。自行理解即可。  
点击**访问控制应用包列表**即可选择应用。  

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/10.jpg)  




## 五。切换代理模式  

![](https://github.com/githubvpn007/Clash-for-Android/blob/main/images/10.jpg) 


## 六。代理模式(一般默认即可)  

    全局（Global）：所有请求直接发往代理服务器  
    规则（Rule）：所有请求根据配置文件规则进行分流  
    直连（Direct）：所有请求直接发往目的地  
    PAC模式:这个模式是根据PAC文件，来判断请求是否要经过代理。  
    
    
## 七。常见的订阅错误报告  

如果遇到以下提示： 

`Invalid Config:yaml:unmarshal errors: line 1:cannot unmarshal !!str c3M6Ly9...`


说明用错了订阅链接，请检查自己是不是复制错了或者多了空格之类的。  

没有 Clash 订阅链接的可以使用 [API](https://bianyuan.xyz/) 来转换订阅链接。  

如果遇到此类提示：  

`Invalid Config:Value for 'Proxy' is invalid:Unexpected null or empty` 


说明你还没买套餐，或者订阅为空。请联系你所在机场的管理员。




## 8.到这里巨差不多 完结  






