# Bilibili直播间挂机助手 for TamperMonkey
在一位用户的建议下将脚本放在这里，但不保证维护

### 删除后更新日志
* 2018-05-12
更新API相关，优化逻辑，尝试规避封号
* 2018-04-30
更新验证码识别算法，修复无法正常领取瓜子的问题
增加新的设置项
* 2018-03-31
更新总督API相关(缺少数据,功能未实装)
* 2018-03-10
更新领取银瓜子的功能

## 以下内容来源于原GreasyFork脚本页面说明

### B站直播间自动签到，领瓜子，参加抽奖（小电视以及活动），完成任务，送礼等（见说明及代码）
这些功能可以自己选择是否开启，默认开启自动签到，领瓜子，完成任务。可点击页面右下角"挂机助手设置"进行设置，设置说明见源代码或设置界面的帮助

#### 自动送礼说明
> 检查当前房间是否为设置的房间，是则开始送礼，否则不送礼（设置为0则自动检查是否有主播头衔，有则自动切换并送礼）
> 检查是否达到亲密度上限，没有则继续送礼，达到上限则停止送礼
> 刷新背包列表，自动计算需要送出的礼物数量，按照背包默认顺序（即过期时间顺序）送礼，直到亲密度已满或背包清空，按照不浪费策略送礼（如：亲密度还可增加9，有亿元但没有辣条，此时不送礼物）
> * 可选：自动切换当前佩戴的头衔
> * 可选：自定义送礼，默认只送辣条
> * 可选：送出今天到期的礼物（无视默认送礼的设置）

#### 已知问题
> 新春抽奖无法在房间号是5位数及以上的直播间正常使用（已解决，但可能导致资源占用过多等问题）

##### 一段时间后将会删除脚本（除夕夜）

#### 节奏风暴抽奖由于验证码识别的技术问题而未实现，会的可以自己实现

#### 开源协议：MIT

#### 更新日志
* 2018-01-09
修复了脚本不能运行的问题
* 2018-01-12
增加了自定义送礼等功能，优化了脚本逻辑
* 2018-01-13
修复了领取宝箱的有关bug
* 2018-01-18
修复了不能正常参加新春抽奖的问题
* 2018-01-20
优化了抽奖功能，调整了浮动提示
* 2018-01-22
增加了可视设置界面和保存设置的功能
增加了新的设置项
移除了使用银瓜子送礼的功能
修复了会自动送出永久期限礼物的bug(未测试)
优化了领取瓜子信息的界面设计
优化了抽奖计时逻辑
* 2018-01-28
调整了设置界面
修改了送礼逻辑
* 2018-02-04
增加了银瓜子兑换硬币的功能
修改了默认设置
调整了设置界面的位置
* 2018-02-10
修复了不能领取银瓜子的问题
* 2018-02-12
解决了不能在任意直播间参加抽奖的问题(实验性)(需在设置中勾选)
* 2018-02-15
修正了节奏风暴有关功能的实现逻辑