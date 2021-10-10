# JD-Assistant

[![version](https://img.shields.io/badge/python-3.4+-blue.svg)](https://www.python.org/download/releases/3.4.0/) 
[![status](https://img.shields.io/badge/status-stable-green.svg)](https://github.com/huaisha1224/jd-assistant)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![star, issue](https://img.shields.io/badge/star%2C%20issue-welcome-brightgreen.svg)](https://github.com/huaisha1224/jd-assistant)

京东抢购助手源代码Fork自[huaisha1124](https://github.com/huaisha1224/jd-assistant/)
-在此基础上进行了修改；运行过程报错的bug已经修复，并修改了时间同步的api接口，但功能并未合并,后续有需要可以合并。


👉 [使用教程请参看Wiki](https://github.com/huaisha1224/jd-assistant/wiki/JD%E6%8A%A2%E8%B4%AD%E5%8A%A9%E6%89%8B)

## 主要功能

- 登陆京东商城（[www.jd.com](http://www.jd.com/)）
  - 手机扫码登录
  - 保存/加载登录cookies (可验证cookies是否过期)
- 商品查询操作
  - 提供完整的[`地址⇔ID`](./area_id/)对应关系
  - 根据商品ID和地址ID查询库存
  - 根据商品ID查询价格
- 购物车操作
  - 清空/添加购物车 (无货商品也可以加入购物车，预约商品无法加入)
  - 获取购物车商品详情
- 订单操作
  - 获取订单结算页面信息 (商品详情, 应付总额, 收货地址, 收货人等)
  - 提交订单（使用默认地址）
    - 直接提交
    - 有货提交
    - 定时提交
  - 查询订单 (可选择只显示未付款订单)
  - 查询本地生活服务订单中的验证码及其状态(验证码是否已消费)
- 其他
  - 商品预约
  - 用户信息查询

## 运行环境

- [Python 3](https://www.python.org/)


安装：
```sh
pip install -r requirements.txt
```
所需文件包列举在 requirements.txt 中
## 使用教程

程序主入口在 `main.py`
