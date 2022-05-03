# SamsClub_buy

上海疫情期间,大家都不好过,物资匮乏,这个脚本初衷是想帮助有困难的人买到物资

请适当使用,把资源留给有需要的人!

## 更新内容

#### 5.3 更新

普通模式和保供模式,增加优惠券功能,getData.py和sam_buy_bao_gong.py运行后可以选择优惠券,请事先确保优惠券可使用

#### 4.30 更新

保供脚本加入白名单文件 whiteList.txt 为空则默认全选,有值则只模糊匹配白名单内的物品 ,例子: ["套餐", "宠物""], 白名单支持热载,修改后保存即可无需重启

#### 4.26 更新

普通模式增加购物车轮询,用于及时更新缺货库存,详见 [常规下单 操作步骤](https://github.com/guyongzx/SamsClub_buy#%E5%B8%B8%E8%A7%84%E4%B8%8B%E5%8D%95-%E6%93%8D%E4%BD%9C%E6%AD%A5%E9%AA%A4)

#### 4.25 更新

执行 sam_buy_bao_gong.py

持续扫描是否有货,有货就加购物车并下单

如果持续上3个套餐,会都下单,最后取消你不需要的

加入barkid参数,如果要bark通知在一开始填入barkid


### 建议不要随意修改sleep时间!!! 并发太高被封ip!!!


## 第一件事: 抓包获取headers里的authtoken,网上搜索手机抓包,推荐charles
## 第二件事: 确保安装了 requests 组件
#### 引入 requests 组件
执行
```bash
pip install --index-url https://pypi.douban.com/simple/ requests
```
## 保供套餐 操作步骤

1: sam_buy_bao_gong.py 类里填写authtoken, barkid(选填)直接执行

## 常规下单 操作步骤

1: normal文件夹下 getData.py 类里填写authtoken

2: 执行getData.py,选择相应地址和仓库

3: 等待提示"购物车加载完成"后,执行order.py即可开始下单

4: 可以不关闭getData.py让其一直运行以保持购物车持续更新


### 此工程参考 https://github.com/azhan1998/sam_buy 

感谢作者付出

## 版权说明

本项目为 GPL3.0 协议，请所有进行二次开发的开发者遵守 GPL3.0协议，并且不得将代码用于商用。

本项目仅供学习交流，严禁用作商业行为，特别禁止黄牛加价代抢等！

因违法违规等不当使用导致的后果与本人无关，如有任何问题可联系本人删除！
