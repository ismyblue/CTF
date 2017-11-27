摘自[http://blog.csdn.net/u012763794/article/details/50959166](http://blog.csdn.net/u012763794/article/details/50959166)
诚挚地感谢作者。

# Web总结
## 基础篇
### 1.直接查看源代码
[http://lab1.xseclab.com/base1_4a4d993ed7bd7d467b27af52d2aaa800/index.php](http://lab1.xseclab.com/base1_4a4d993ed7bd7d467b27af52d2aaa800/index.php)
>按F12 查看源代码，答案出

### 2.修改或添加HTTP请求头
常见的有：
Referer来源伪造
X-Forwarded-For：ip伪造
User-Agent：用户代理（就是用什么浏览器什么的）
[题目](http://lab1.xseclab.com/base6_6082c908819e105c378eb93b6631c4d3/index.php)
>使用Burpsuite抓http包，修改http包里浏览器Mozilla为HAHA,重发一遍，得到key 恭喜您，成功安装HAHA浏览器！key is: meiyouHAHAliulanqi


Accept-Language：语言
[题目](http://lab1.xseclab.com/base1_0ef337f3afbe42d5619d7a36c19c20ab/index.php)
>用burpsuite抓包后修改Accept-Language:en或者en-US,重新发送，key is: *(TU687jksf6&*

[题目](http://ctf1.shiyanbar.com/basic/header/)
>Accept-Language 改成zh-hk

Cookie的修改
[题目](http://lab1.xseclab.com/base9_ab629d778e3a29540dfd60f2e548a5eb/index.php)
>抓http包，在Cookie把Login=0改成Login=1
>key is: yescookieedit7823789KJ

### 3.查看HTTP请求头或响应头


[题目](http://lab1.xseclab.com/base7_eb68bd2f0d762faf70c89799b3c1cc52/index.php)
>直接查看httpRespon包里面就有Key: kjh%#$#%FDjjj

[题目](http://ctf1.shiyanbar.com/basic/catch/)


### 4.302跳转的中转网页有信息
[题目](http://lab1.xseclab.com/base8_0abd63aa54bef0464289d6a42465f354/index.php)
>第一个网页，有个链接，点击链接抓包，response里面有个链接，进去有key: ohHTTP302dd