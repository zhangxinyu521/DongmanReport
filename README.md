# DongmanReport
DongmanReport是一款适用于chatgpt-on-wechat项目的新闻资讯类插件，调用天聚数行的API接口，通过代码加工后生成文字版和图片版的AI日报。
该插件是原来的DongmanReport_pic图片版和DongmanReport_txt文字版AI日报插件的整合版本，安装此插件之前可将另外两个先行卸载。

该插件安装需要配置环境。具体的使用教程如下：

## 一. 安装Html渲染所必需的环境
1. 安装playwright：在服务器终端执行以下命令 ：pip install playwright
2. 安装chromium：在服务器终端执行以下命令 ：playwright install chromium
3. 安装字体：在服务器终端执行以下命令 ：yum groupinstall "fonts"

## 二. 获取TIAN_API_KEY并申请接口
1.在天聚数行API接口网站注册账号并登录，官网链接：https://www.tianapi.com

2.点击网站首页的“控制台”进入个人主页，点击左上角“数据管理”➡️“我的密钥KEY”,复制默认的APIKEY备用。

3.在上述网站首页“一键搜索”栏搜索“动漫资讯”，跳转至对应详情页点击“申请接口”，然后点击“在线测试”测试接口是否正常。普通用户每天可免费调用100次。

## 三. 安装插件和配置config文件
1.下载到plugins文件夹中

2.进入config文件配置第一步操作中获取的TIAN_API_KEY。

3.重启chatgpt-on-wechat项目。

4.在微信机器人聊天窗口输入#scanp 命令扫描新插件是否已添加至插件列表

5.输入#help dongmanReport查看帮助信息，返回相关帮助信息则表示插件安装成功。

## 四. 使用样例
![alt text](f4b96a78c3a35e3d9a07815540af8dd.png)

PS:手动修改templates文件夹中news_template.html文件的第123行代码可自定义卡片下方的签名。


本插件根据Lingyuzhou的AIReport（https://github.com/Lingyuzhou111/AIReport.git
）
改编而来，感谢Lingyuzhou的贡献。