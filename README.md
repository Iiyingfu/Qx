# Quantumult X小白配置 制作 by Orz-3 TG频道：t.me/Orzmini 2024/7/5更新

[general]
network_check_url = http://www.apple.com/library/test/success.html
server_check_url=http://cp.cloudflare.com/generate_204
dns_exclusion_list = *.cmpassport.com, *.jegotrip.com.cn, *.icitymobile.mobi, id6.me, *.pingan.com.cn, *.cmbchina.com
geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/Orz-3/Orz-3/master/QuantumultX/IP.js
resource_parser_url = https://cdn.jsdelivr.net/gh/KOP-XIAO/QuantumultX@master/Scripts/resource-parser.js
excluded_routes=239.255.255.250/32
fallback_udp_policy = reject
udp_drop_list = 443
icmp_auto_reply = true

[dns]
no-ipv6
server=119.29.29.29
server=180.184.1.1
server=223.5.5.5
address=/mtalk.google.com/108.177.125.188
server=/dl.google.com/119.29.29.29
server=/dl.l.google.com/119.29.29.29
server=/update.googleapis.com/119.29.29.29
server=/*.dl.playstation.net/119.29.29.29
circumvent-ipv4-answer = 127.0.0.1, 0.0.0.0, 61.160.148.90, 182.43.124.6, 124.236.16.201, 39.102.194.95, 36.135.17.248, 36.135.82.110, 39.105.1.17, 39.130.181.72, 39.130.181.73, 39.173.74.185, 47.92.198.202, 111.22.226.1, 111.28.0.32, 111.31.192.110, 111.44.246.131, 111.56.127.216, 111.63.132.170, 112.15.232.43, 112.17.14.211, 112.54.50.50, 117.156.25.11, 117.187.10.42, 120.202.17.103, 120.209.204.204, 120.222.19.204, 121.4.135.105,183.203.36.19, 183.207.72.18, 183.213.92.2, 183.220.145.129, 183.252.183.9, 211.137.133.69, 211.138.218.190, 211.139.25.61, 211.139.145.129, 218.201.25.129, 218.201.25.130, 218.203.122.98, 221.130.39.3
circumvent-ipv6-answer = ::

[policy]
static=全球加速, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Global.png
static=苹果服务, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Apple.png
static=港台番剧, 香港节点, 台湾节点, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/StreamingSE.png
static=国际媒体, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Streaming.png
static=电报代理, 狮城节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Telegram.png
static=黑白名单, 香港节点, 台湾节点, 日本节点, 韩国节点, 狮城节点, 美国节点, 特殊节点, proxy, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Final.png
static=特殊节点, server-tag-regex=^(?!.*(港|台|日|韩|坡|美|HK|US|TW|JP|KR|SG|Hong|Tai|Japan|Korea|Singapore|States)), img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/Static.png
url-latency-benchmark=香港节点, server-tag-regex=(?=.*(港|HK|(?i)Hong))^((?!(台|日|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/HK.png
url-latency-benchmark=台湾节点, server-tag-regex=(?=.*(台|TW|(?i)Taiwan))^((?!(港|日|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/TW.png
url-latency-benchmark=日本节点, server-tag-regex=(?=.*(日|JP|(?i)Japan))^((?!(港|台|韩|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/JP.png
url-latency-benchmark=韩国节点, server-tag-regex=(?=.*(韩|韓|朝|KR|(?i)Korea))^((?!(港|台|日|新|美)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/KR.png
url-latency-benchmark=狮城节点, server-tag-regex=(?=.*(新|狮|獅|SG|(?i)Singapore))^((?!(港|台|日|韩|兰|美)).)*$, check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/SG.png
url-latency-benchmark=美国节点, server-tag-regex=(?=.*(美|US|(?i)States|American))^((?!(港|台|日|韩|新)).)*$, check-interval=600, tolerance=0, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Color/US.png
[server_remote]



[filter_remote]
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Direct+.list, tag=直连修正, force-policy=direct, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Reject/Advertising.list, tag=广告拦截, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Reject/Tracking.list, tag=隐私保护, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Streaming/Video/TikTok.list, tag=海外抖音, force-policy=全球加速, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Google/GoogleVoice.list, tag=谷歌语音, force-policy=美国节点, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Telegram.list, tag=电报代理, force-policy=电报代理, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Streaming/!CN.list, tag=国际媒体, force-policy=国际媒体, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Streaming/CN.list, tag=港台番剧, force-policy=港台番剧, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Proxy.list, tag=全球加速, force-policy=全球加速, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Apple/Apple.list, tag=苹果服务, force-policy=苹果服务, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Direct.list, tag=国内网站, force-policy=direct, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/WeChat.list, tag=微信直连, force-policy=direct, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Proxy+.list, tag=代理修正, force-policy=proxy, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/Cats-Team/AdRules/main/qx.conf, tag=广告终结者, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Ruleset/Extra/Reject/Advertising.list, tag=广告拦截, force-policy=reject, update-interval=172800, opt-parser=true, enabled=true

[rewrite_remote]
[https://raw.githubusercontent.com/Peng-YM/Sub-Store/master/config/QX.snippet, tag=Sub Store, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.conf, tag=BoxJs, update-interval=172800, opt-parser=true, enabled=true
](https://raw.githubusercontent.com/Peng-YM/Sub-Store/master/config/QX.snippet, tag=Sub Store, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.conf, tag=BoxJs, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/TestFlightDownload.conf , tag=TestFlight区域限制解除, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/TikTok.conf, tag=Tiktok解锁, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Module/Block/YouTubeAds.sgmodule, tag=YouTube去广告, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ddgksf2013/Rewrite/master/AdBlock/StartUp.conf, tag=墨鱼去开屏, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/app2smile/rules/master/module/tieba-qx.conf, tag=贴吧去广告, update-interval=172800, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ConnersHua/RuleGo/master/Surge/Module/Block/Advertising.sgmodule, tag=神机去广告, update-interval=172800, opt-parser=true, enabled=true)
https://raw.githubusercontent.com/zlking02/Emby/main/Module/Premiere/QuanX.conf, tag=Emby Premiere, update-interval=86400, opt-parser=false, enabled=true

# ======= 会员解锁 ======= #
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/Bilibili.conf, tag=哔哩哔哩广告净化@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/UnlockVip/Spotify.conf, tag=Spotify音乐VIP[音质≤高]@app2smile, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/dev/raw/master/ForOwnUse.conf, tag=墨鱼专属VIP@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true

# ======= 广告净化 ======= #
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/StartUp.conf, tag=墨鱼去开屏2.0@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/CaiYunAds.conf, tag=彩云天气净化@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://gist.githubusercontent.com/ddgksf2013/d43179d848586d561dbb968dee93bae8/raw/Zhihu.Adblock.js, tag=知乎净化助手@ddgksf2013, update-interval=86400, opt-parser=true, enabled=true
https://github.com/app2smile/rules/raw/master/module/tieba-qx.conf, tag=百度贴吧去广告@app2smile, update-interval=86400, opt-parser=false, enabled=false
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/Applet.conf, tag=微信小程序去广告@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/YoutubeAds.conf, tag=油管去广告@Maasea, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/Weibo.conf, tag=微博去广告@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/Ximalaya.conf, tag=喜马拉雅去广告[卸载重装]@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/Amap.conf, tag=高德地图净化[卸载重装]@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/NeteaseAds.conf, tag=网易云净化@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true

# ======= 网页优化 ======= #
https://github.com/ddgksf2013/Rewrite/raw/master/Html/Q-Search.conf, tag=Safari超级搜索@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/Html/Douban.conf, tag=豆瓣网页观影快捷跳转@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://github.com/ddgksf2013/Rewrite/raw/master/Html/General.conf, tag=Google重定向@DivineEngine, update-interval=86400, opt-parser=false, enabled=true

# ======= 功能增强 ======= #
https://github.com/ddgksf2013/Rewrite/raw/master/AdBlock/XiaoHongShu.conf, tag=小红书净化+去水印@ddgksf2013, update-interval=86400, opt-parser=false, enabled=true
https://gist.githubusercontent.com/ddgksf2013/f43026707830c7818ee3ba624e383c8d/raw/baiduCloud.adblock.js, tag=百度网盘净化@ddgksf2013, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/ddgksf2013/Rewrite/master/Function/UnblockURLinWeChat.conf, tag=微信解锁被屏蔽的URL@zZPiglet, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.conf, tag=BoxJS商店版@chavyleung, update-interval=86400, opt-parser=false, enabled=false
[server_local]

[filter_local]
host-suffix, missav.com, 全球加速
host-suffix, 91md.me, 全球加速
host-suffix, imyyds.com, 全球加速
host-suffix, xchina.co, 全球加速
host-suffix, rou.video, 全球加速
host-suffix, hlj.fun, 全球加速
host-suffix, local, direct
ip-cidr, 192.168.0.0/16, direct
ip-cidr, 10.0.0.0/8, direct
ip-cidr, 172.16.0.0/12, direct
ip-cidr, 127.0.0.0/8, direct
ip-cidr, 100.64.0.0/10, direct
ip-cidr, 224.0.0.0/4, direct
ip6-cidr, fe80::/10, direct
geoip, cn, direct
final, 黑白名单

[rewrite_local]
^https?:\/\/(www.)?(g|google)\.cn url 302 https://www.google.com

[task_local]
event-interaction https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/streaming-ui-check.js, tag=流媒体解锁查询, img-url=arrowtriangle.right.square.system, enabled=true

[http_backend]

[mitm]
skip_validating_cert = true
hostname = www.google.cn
