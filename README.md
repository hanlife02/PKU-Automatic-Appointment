# PKU_Automatic_Appointment

A script for automatic appointments for Peking University students.<br><br>
一个供北大学生使用的自动预约脚本

## Instructions
这是一个使用浏览器驱动可视化自动预约的脚本，使用的原因是方便截图。<br>~~(绝对不是因为我只会这个)~~<br><br>
**如果你不想绑定手机令牌，看到这里就可以退出了(x**<br><br>
这个脚本用起来还挺麻烦的，如果你和我一样懒的话，不妨自己写一个脚本用（绝对比这个要好hh<br><br>
最后，如果你好奇的话，也可以试一试这个。<br>

## Installation

### Prerequisites
- Python 3.x
- EdgeDriver

### Libraries
- selenium
- python-dotenv
- pyotp

If you don't have these libraries
```
pip install selenium python-dotenv pyotp
```

## Usage

### 壹 · 准备
<br>
① 使用`Edge`并安装`edgedriver`（如果使用其它浏览器，也可更改为相应的驱动）<br><br>
https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/?form=MA13LH<br><br>
此网站下载`edgedriver`<br><br>
并复制`msedgedriver.exe`的路径，后续配置环境变量会用到<br><br>

② 确保你的`python`环境已经存在<br><br>

③ 已经安装上述`Libraries`的三个库<br><br>

④ 一个清醒的大脑

----

### 贰 · 注意
<br>
① 建议门户绑定微信公众号，弹窗有一定几率导致失败(经测试失败概率不高，但仍然存在）<br><br>
②后面的忘了，想起来再加hh，如果碰到问题，欢迎及时反馈，十分感谢！<br><br>

------

### 叁 · 流程
<br>

① **克隆此仓库到本地**<br>

[仓库地址](https://github.com/hanlife02/PKU_Automatic_Appointment)<br><br>
![示例图片1](https://hanlife02.com.cn/api/v2/objects/file/gt9l6pjzwwu7a5as5a.png)<br><br>

② **绑定手机令牌**<br><br>
按照 [此处](https://iaaa.pku.edu.cn/iaaa/resources/help/otpHelp.html) 的教程，使用 FreeOTP 绑定手机令牌，并获得二维码的URL<br><br>
（URL的获取只需要用微信识别二维码，并复制链接即可）<br><br>
类如otpauth://totp/iaaa.pku.edu.cn:23********?secret=NQG32\*\*\*\*\*\*\*\*\*\*\*&issuer=iaaa.pku.edu.cn<br><br>
复制`secret`的内容，后续配置环境变量会用到<br><br>

③ **修改环境变量**<br><br>
按照要求修改`.env`即可<br><br>

④ **运行 `main.py`**<br><br>
见到下图即运行成功<br><br>
![](https://hanlife02.com.cn/api/v2/objects/file/2dhy73n26f3nd2ct6k.png)
<br><br>
运行成功后，浏览器窗口将在5分钟后自动关闭，请及时截图保存信息。

## 免责声明
  1.本仓库严禁用于任何商业用途！<br><br>
  2.申请信息与事实不符产生的一切后果本人均不负责!<br><br>
  3.网络状况不稳定导致的预约失败本人均不负责！<br><br>
