# VerifyCode
Python生成随机验证码模块

## 安装

```bash
git clone https://github.com/TengTengCai/VerifyCode.git
```

该模块依赖Pillow图形处理库, 使用之前请先安装Pillow

```bash
pip install pillow
```

## 使用

直接引入模块即可

```python
from VerifyCode import VerifyCode  # 导人包

vcode = VerifyCode()  # 生成验证码对象

str_code = vcode.verify_code  # 获取生成的字符串验证码

image_code = vcode.verify_image  # 获取生成的图片验证码
```

## 参数

```python
VerifyCode(length=4, width=160, height=50, font_size=40)
"""
验证码初始化方法
    
:param length: 验证码长度 默认length=4
:param width: 验证码图片宽度 默认width=160
:param height: 验证码图片高度 默认height=50
:param font_size: 字体大小 默认font_size=40
"""
```

