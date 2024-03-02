# CyWr110

## 致敬开源精神 净化网络环境

### 不只是 QuantumultX 脚本

![GitHub contributors](https://img.shields.io/github/contributors/fmz200/wool_scripts?style=for-the-badge)
![GitHub stars](https://img.shields.io/github/stars/fmz200/wool_scripts?color=ffd700&style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/fmz200/wool_scripts?color=60c5ba&style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/fmz200/wool_scripts?color=1E90FF&style=for-the-badge)
![Github Codelines](https://img.shields.io/tokei/lines/github/fmz200/wool_scripts?style=for-the-badge)
![GitHub](https://img.shields.io/github/license/fmz200/wool_scripts?style=for-the-badge)
[![](https://img.shields.io/badge/-t.me/quguanggao-3db6f1?style=for-the-badge&logo=Telegram&logoColor=2ca5e0)](https://t.me/lanjieguanggao)

<br />

<p align="center">
  <a href="https://github.com/fmz200/wool_scripts">
    <img src="pic/logo/logo05.png" alt="Logo" width="396" height="109">
  </a>
</p>

---

## ✅ 一些说明：

▶️ 由于张军大佬隐退，所以我接管进行日常更新，故本库中存储的就是张军大佬的且是最新的配置，不要再问了。

▶️ 每个配置文件的开头部分都有使用说明，且每个文件夹中都有文件名为`00-How-To-Use-xxx.md`的教程文件，使用前请先看说明。

▶️ 如果你在使用过程中有问题欢迎提交PR或ISSUE，也可进群交流，群链接在下方。

▶️ 本库中大部分内容收集于互联网开源项目，在此对原作者表示衷心的感谢。同时，我们谴责将他人内容标注为自己原创的行为。

▶️ 使用本项目中的内容所造成的一切后果，均由使用者承担。

▶️ 本项目中的内容请不要在中国大陆的任何平台传播。

▶️ 交流群组：张军配置👉🏻[苹果iOS去广告交流群](https://t.me/lanjieguanggao)，备用群组👉🏻[去广告交流备用|群组](https://t.me/ddgksf2021_chat)。

---

## 🚸 常见问题

### 1️⃣ 我为什么指定了抖音的分流到国外，评论视频却显示“IP未知”

> 答：抖音与其他软件判断IP归属地的方式不同，抖音需要家庭宽带IP（又叫住宅IP）才能生效，而现在的大部分机场都是机房的IP，所以评论视频就显示IP未知。
> 如果你不知道自己抖音分流的IP是不是家宽，可以访问[https://ipinfo.io](https://ipinfo.io/) 查看，在`asn`
> 信息中如果你看到`type:
"isp"`那就是家庭宽带，其他值（比如：hosting，business）都不是家宽。

常见的抖音分流有：
> https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/DouYin/DouYin.list

### 2️⃣ 为什么有些软件明明很热门，却没有人做去广告的规则

> 答：对于一些软件，如果整个域名都是广告，则可以直接reject整个域名去广告，但是大部分广告都和非广告内容一起返回，这就需要对响应体（response-body）进行解析来去掉其中的广告内容。
> 解析响应体的前提条件是访问的域名可以MITM（MAN-IN-THE-MIDDLE：中间人攻击），但是有些域名禁止了MITM，所以无法对响应体进行解析去广告。

已知不能或不能完全去广告的app有：
> 抖音，今日头条、蜂巢、滴答清单 Taio、小米运动、有条下载、Fileball、万年历、豆瓣（信息流）、虎牙直播、货拉拉、番茄小说、凯叔讲故事、
> 什么值得买、广东移动、淘宝、银行类（绝大部分）。

---

## 🍑 开始使用

### 1️⃣ QuantumultX配置

> 📍 借助 [QuanX官方Github地址](https://github.com/crossutility/Quantumult-X)，你可以更快地理解QX配置。
>
> 📍 配置前建议先看一看 [QuanX 小白配置图文教程](./QuantumultX/How-To-Use.md)，这里包括了从准备配置到配置完成的详细说明。
>
> 📍 这里也有**Hell Cell**大佬的[视频教程](https://youtu.be/e8E8dtFaFUk)，强烈建议小白在配置前认真观看几遍！

| #  | 配置类型    | 配置名称          | 配置链接                                                                                                                        | 作者                                  | 特别说明                           | 使用教程                                                   |
|----|---------|---------------|-----------------------------------------------------------------------------------------------------------------------------|-------------------------------------|--------------------------------|--------------------------------------------------------|
| 01 | 全局配置    | `懒人配置`        | [QuanX.conf](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/config/QuanX.conf)                    | [fmz200](https://github.com/fmz200) | 下载此文件会覆盖原本所有配置                 | [点击查看](./QuantumultX/config/00-How-To-Use-Config.md)   |
| 02 | 重写      | `去广告合集`       | [chongxie.txt](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/chongxie.txt)                 | [fmz200](https://github.com/fmz200) | 去广告合集，不包含微博                    | [点击查看](./QuantumultX/rewrite/00-How-To-Use-Rewrite.md) |
| 03 | 重写      | `微博去广告`       | [weibo.snippet](https://raw.githubusercontent.com/RuCu6/QuanX/main/Rewrites/Cube/weibo.snippet)                             | [RuCu6](https://github.com/RuCu6)   | 包含净化，去除了一些不需要的模块               | [点击查看](./QuantumultX/rewrite/00-How-To-Use-Rewrite.md) |
| 05 | 重写      | `微博去广告`       | [fmz200_weibo.snippet](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/fmz200_weibo.snippet) | [fmz200](https://github.com/fmz200) | 自用的配置                          | [点击查看](./QuantumultX/rewrite/00-How-To-Use-Rewrite.md) |
| 06 | 重写      | `获取cookie合集`  | [cookies.snippet](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/cookies.snippet)           | [fmz200](https://github.com/fmz200) | 包含NobyDa，chavyleung，Sunert等    | 暂无                                                     |
| 07 | 分流      | `去广告合集`       | [fenliuxiu.list](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/fenliuxiu.list)              | [fmz200](https://github.com/fmz200) | 无                              | [点击查看](./QuantumultX/filter/00-How-To-Use-Filter.md)   |
| 08 | 分流      | `分流修正`        | [fenliuxiuzheng.list](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/fenliuxiuzheng.list)    | [fmz200](https://github.com/fmz200) | 无                              | [点击查看](./QuantumultX/filter/00-How-To-Use-Filter.md)   |
| 09 | 分流      | `屏蔽苹果系统更新`    | [apple.snippet](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/apple.snippet)                | [fmz200](https://github.com/fmz200) | 有效性未知                          | [点击查看](./QuantumultX/filter/00-How-To-Use-Filter.md)   |
| 10 | 分流      | `OpenAI分流`    | [OpenAI.snippet](https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/OpenAI.snippet)              | [fmz200](https://github.com/fmz200) | 初始版本，有问题欢迎反馈                   | [点击查看](./QuantumultX/filter/00-How-To-Use-Filter.md)   |
| 11 | BoxJS订阅 | `BoxJS订阅`     | [fmz200.boxjs.json](https://raw.githubusercontent.com/fmz200/wool_scripts/main/boxjs/fmz200.boxjs.json)                     | [fmz200](https://github.com/fmz200) | 先查看使用教程                        | [点击查看](https://docs.boxjs.app)                         |
| 12 | Task订阅  | `Task订阅`      | [fmz200_gallery.json](https://raw.githubusercontent.com/fmz200/wool_scripts/main/boxjs/fmz200_gallery.json)                 | [fmz200](https://github.com/fmz200) | 需要先获取cookie或token再运行           | 暂无                                                     |
| 13 | icons图标 | `icons图标`     | [icons-all.json](https://raw.githubusercontent.com/fmz200/wool_scripts/main/icons/icons-all.json)                           | [fmz200](https://github.com/fmz200) | 包含APP，机场，LPL等大量图标              | 暂无                                                     |
| 14 | 重写      | `App&小程序净化合集` | [cleanup.snippet](https://github.com/fmz200/wool_scripts/raw/main/QuantumultX/rewrite/cleanup.snippet)                      | [fmz200](https://github.com/fmz200) | 常见的微信小程序净化                     | 暂无                                                     |

> ⚠️ 当远程图标更新时如果你的图表库不更新多半是缓存的问题，请手动清理图标缓存(`点击右下角风车->划到最下面->选择其他设置->找到资源模块`，选择`删除图片缓存`)，并重启 Quantumult X，远程图标会重新下载并生效。

### 2️⃣ Surge配置

> 📍 你可以借助转换工具将重写和分流添加到Surge中，项目地址如下：[Surge](https://github.com/chengkongyiban/Surge)

| #  | 配置类型 | 配置名称       | 配置链接                                                                                             | 作者                                  | 特别说明         | 使用教程 |
|----|------|------------|--------------------------------------------------------------------------------------------------|-------------------------------------|--------------|------|
| 01 | 分流   | `OpenAI分流` | [OpenAI.list](https://raw.githubusercontent.com/fmz200/wool_scripts/main/Surge/rule/OpenAI.list) | [fmz200](https://github.com/fmz200) | 初始版本，有问题欢迎反馈 | 无    |

### 3️⃣ Loon配置

> 📍 你可以借助转换工具将重写和分流添加到Loon中，项目地址如下：[Loon](https://github.com/chengkongyiban/Loon)
> 
> 📍 具体步骤为：
> 
> 1、安装`QX或Surge重写&规则集转Loon`插件：
> ```
> https://raw.githubusercontent.com/chengkongyiban/Loon/main/Loon-Gallery/Rewrite_to_Loon.plugin
> ```
> 
> 2、安装好上面的插件以后，即可把QX的重写和分流安装到Loon上：
> 
> ⚠️ 注意：QX重写链接需要在原链接上加上`qx`，分流链接需要加上`r_parser.list`，以便转换插件识别进行解析
> 
> 2.1、添加QX的重写：⚠️ 注意，安装到Loon的`插件`模块
> 
> 🍒 去广告重写合集
> ```
> https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/chongxie.txtqx
> ```
> 🍒 微博去广告
> ```
> https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/weibo.snippetqx
> ```
> 🍒 获取cookie合集
> ```
> https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/rewrite/cookies.snippetqx
> ```
> 2.2、添加QX的分流：⚠️ 注意，安装到Loon的`规则`模块
> 
> 🍒 去广告分流合集
> ```
> https://raw.githubusercontent.com/fmz200/wool_scripts/main/QuantumultX/filter/fenliu.listr_parser.list
> ```

| #  | 配置类型   | 配置名称     | 配置链接                                                                                                | 作者                                  | 特别说明                 | 使用教程 |
|----|--------|----------|-----------------------------------------------------------------------------------------------------|-------------------------------------|----------------------|------|
| 01 | Task订阅 | `Task订阅` | [loon.task.scripts](https://github.com/fmz200/wool_scripts/raw/main/Loon/scripts/loon.task.scripts) | [fmz200](https://github.com/fmz200) | 需要先获取cookie或token再运行 | 暂无   |

### 4️⃣ ShadowRocket配置

> 📍 你可以借助转换工具将重写和分流添加到ShadowRocket中，项目地址如下：[ShadowRocket](https://github.com/chengkongyiban/shadowrocket)

### 5️⃣ Stash配置

> 📍 你可以借助转换工具将重写和分流添加到Stash中，项目地址如下：[stash](https://github.com/chengkongyiban/stash)

---

## 🧲 写着玩的

> 📍 配置前建议先看一看脚本内说明，不要张口就问。

| # | 名称    | 作用                                   | 链接（长按可复制链接）                                                             | 作者            | 特别说明                                                       | 使用教程  |
|---|-------|--------------------------------------|-------------------------------------------------------------------------|---------------|------------------------------------------------------------|-------|
| 1 | 节点重命名 | `在SubStore内使用脚本对订阅节点重命名，落地IP检测，节点去重` | [cname.js](https://raw.githubusercontent.com/Keywos/rule/main/cname.js) | @key @小一 @奶茶姐 | 针对有些机场名称乱写的现象对节点重新命名，使用前查看脚本内使用说明，只支持Loon和Surge，QX本身不支持此功能 | 脚本内查看 |

---

## 🧚‍♂️ 特别鸣谢

- [@28413761](https://github.com/28413761)(张军本人)
- [@app2smile](https://github.com/app2smile)
- [@blackmatrix7](https://github.com/blackmatrix7)
- [@chavyleung](https://github.com/chavyleung)
- [@chengkongyiban](https://github.com/chengkongyiban)
- [@DivineEngine](https://github.com/DivineEngine)
- [@I-am-R-E](https://github.com/I-am-R-E)
- [@Keywos](https://github.com/Keywos)
- [@kokoryh](https://github.com/kokoryh)
- [@KOP-XIAO](https://github.com/KOP-XIAO)
- [@lodepuly](https://gitlab.com/lodepuly)
- [@NobyDa](https://github.com/NobyDa)
- [@Orz-3](https://github.com/Orz-3)
- [@RuCu6](https://github.com/RuCu6)
- [@Tartarus2014](https://github.com/Tartarus2014)
- [@zmqcherish](https://github.com/zmqcherish)

## 🧚‍♀️ 欢迎星标 🌟

![Star](https://api.star-history.com/svg?repos=fmz200/wool_scripts&type=Date)

### 🧚‍♀️ 访问量统计

![Visitor Count](https://profile-counter.glitch.me/fmz200/count.svg)

