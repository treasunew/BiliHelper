[![Treasunew's GitHub stats](https://github-readme-stats.vercel.app/api?username=treasunew&show_icons=true&theme=radical)](https://github.com/anuraghazra/github-readme-stats)  
![visitors](https://visitor-badge.glitch.me/badge?page_id=fantingsheng.fantingsheng&left_color=green&right_color=red)
# BiliHelper
A tool to upgrade bilibili's level  
本项目是之前大佬写的，但是后面删库跑路了，我刚好下载下来了，所以再发一下，给大家使用
偶尔会发一些好玩的，TG频道[TelegramGroup](https://t.me/PorterTree)
## 教程
1. 首先把项目下载下来，然后解压会得到三个文件  
  - Bili.sh  
  - config.json  
  - [^java包]: BILIBILI-HELPER-v2.1.0.jar
2. 打开我们的sftp工具，将三个文件上传到/root/ql/scripts目录下
3. 然后打开青龙面板，点击任务管理加入一个任务
  - 命令: task Bili.sh
  - cron: 0 12 * * * 自己随意更改
## 配置文件
### TaskConfig
1. 部分变量介绍

| 变量名 | 参数 | 描述 |
|:----:| :----: | :----: |
| biliCookies | COOKIE | 通过浏览器获取即可 |
| skipDailyTask | true/false | 是否跳过每日任务 |
| matchGame | true/false | 预测比赛 |
| showHandModel | true/false | 俺也不知道 |
| predictNumberOfCoins | 5 | 预测比赛投的硬币数量 |
| minimumNumberOfCoins | 0 | 最小的硬币数量，我也不知道有啥用 |
| taskIntervalTime | 20 | 任务时间间隔 |
| numberOfCoins | 5 | 投币数量 |
| coinAddPriority | 1 | 优先级，我也不是很懂，默认就行 |
| reserveCoins | 100 | 预留的硬币数，账户最低硬币数 |
| selectLike | 未知 | 我也不知道是什么 |
| monthEndAutoCharge | true/false | 每月是否自动充电 |
| giveGift | true/false | 是否自动送礼物 |
| silver2Coin | true/false | 银瓜子是否自动兑换硬币 |
| upLive | 未知 | 我也不知道是什么 |
| chargeForLove | UID | 充电的对象UID |
| chargeDay | 28 | 充电的时间 |

2. 变量解释
  - biliCookies  自己通过浏览器的开发者工具获取，将一整段COOKIE放进去即可
  - selectLike 我也不知道是什么
  - upLive 我也不知道是什么
  - skipDailyTask 跳过每日任务，自己选择
  - monthEndAutoCharge 月末自动充电
  - giveGift 送礼物
  - silver2Coin 银瓜子兑换硬币
  - chargeForLove 充电的对象，自己填UID
  - chargeDay 每月充电的时间，一般都是月末那一天
  
### pushConfig
| 变量名 | 参数 | 描述 |
|:----:| :----: | :----: |
| SC_KEY | xxxx | sever酱老版本的sendkey，可关注公众号方糖获取 |
| SCT_KEY | xxxx | sever酱新版本的sendkey，可关注公众号方糖获取 |
| TG_BOT_TOKEN | 368236:ninivqofwonvnwv | TG机器人的token，可通过botfather创建机器人并获取 |
| TG_USER_ID | 1916361 | 通过Get My Id 机器人获取 |
| TG_USE_CUSTOM_URL | false | 默认即可 |
| DING_TALK_URL | https://xxxx | 自己通过创建钉钉群机器人获取 |
| DING_TALK_SECRET | xxxxxx | 创建机器人产生的秘钥 |
| PUSH_PLUS_TOKEN | IUN2767387833 | pushplus的个人TOKEN |
| WE_COM_GROUP_TOKEN | 企业微信的Token | 通过创建企业微信群获取 |
| WE_COM_APP_CORPID | 企业ID | 创建企业之后去官网查看 |
| WE_COM_APP_CORP_SECRET | 企业秘钥 | 创建企业之后去官网查看 |
| WE_COM_APP_AGENT_ID | 企业应用ID | 创建应用之后可以查看 |
| WE_COM_APP_MEDIA_ID | 媒体ID | 通过企业应用的素材库上传即可获得链接且查看mediaID |
| WE_COM_APP_TO_USER | @all | 给谁发消息，也可以填ID，@all是指给所有人发消息 |
| PROXY_HTTP_HOST | http://xxxxxx | 一般服务器没有代理的时候就自己找个http代理填进去就行 |
| PROXY_SOCKET_HOST | xxxxxxx | 代理的秘钥 |
| PROXY_PORT | 0000 | 代理端口 |
## 总结
1. 库里的东西是之前大佬写的，我是纯搬运，如果大佬不想我公开这个项目，可以联系我
2. 因为写文档我还不太熟练，如果有写错的地方，大家可以提issue
3. 如果运行有任何问题，大家不要提issue，我也解决不了
4. 大家尽量不要Fork
5. 因为忘了从哪儿下载的了，就不提原作者了
