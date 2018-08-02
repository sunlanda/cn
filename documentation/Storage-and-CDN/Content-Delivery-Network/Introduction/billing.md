# 计费说明
## 普通预付费方式

客户需预先在京东云账户下充值；

支持流量计费和带宽峰值流量计费两种模式，默认采用流量计费：

按天计费，计费周期为每天0时-24时，每天6时，进行前一天的账单结算；

1)   流量计费：按实际使用的流量计费，单位为GB，每日扣费、按月阶梯，每次计费时，对用户在本次计费周期中产生的流量进行自然月阶梯计费。


2)   带宽峰值计费：按使用的带宽峰值计费，每5分钟统计一个带宽，每天共统计288个点，每次计费时，对用户在本次计费周期中的带宽最大值(带宽峰值)进行日阶梯计费。


## 大客户后付费方式

为满足业务规模较大客户的灵活计费要求，京东云CDN也支持按95带宽峰值或月度总流量，以月结后付费的模式计费。客户先使用服务、后付费，每月1号出上个月的用量账单，并按线下合同约定条款付费，具体情况可与京东云商务洽谈。

95带宽峰值计费说明：

95带宽峰值计费按自然月结算，在一个自然月内，取每5分钟有效带宽值进行降序排列，然后把带宽数值最高的5%的点去掉，剩下的最高带宽就是95带宽峰值计费值。

以一月30天为例，每5分钟1个带宽取值点，每小时12个取值点，每月取值点数为 12 x 24 x 30 = 8640个。将所有的点按带宽数值降序排列，去掉前5%的点 8640 x 5% = 432 个点，即第433个点为计费点。