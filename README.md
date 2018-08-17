# qqlib3

Python3


模拟QQ登陆第三方网站，获取登录状态下的cookie

当前遇到验证码会报错，腾讯更改了滑块图片地址和js加密算法。无验证码可正常登陆，滑块缺口算法依然可用

欢迎推送最新js滑块加密算法

Examble：

from qqlib3 import QQ

qq = "190758586"

p = 'xxxxxxxxxx'

third_url = 'http://www.58pic.com/index.php?m=login&a=snsLogin&type=qq&isRedirect=1'

qq = QQ(third_url=third_url, qq=q, password=p)

print(qq.login())

