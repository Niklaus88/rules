# Clash / Mihomo 分流规则镜像仓库

本仓库为 Clash / Mihomo 系列配置及相关客户端提供分流规则集镜像备份，主要收录常用海外服务、流媒体及应用规则，防止上游仓库异动或删库导致订阅分流失效。

---

## 规则集列表

### 1. 核心应用与流媒体分流（项目主力引用）

| 规则名称 | 适用策略组 | 规则类型 | CDN 镜像链接 (推荐) | GitHub 直连 |
| :--- | :--- | :--- | :--- | :--- |
| **YouTube.txt** | YouTube | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/YouTube.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/YouTube.txt) |
| **Netflix.txt** | Netflix | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Netflix.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/Netflix.txt) |
| **Spotify.txt** | Spotify | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Spotify.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/Spotify.txt) |
| **AI.txt** | AI | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/AI.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/AI.txt) |
| **TikTok.txt** | TikTok | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/TikTok.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/TikTok.txt) |
| **Microsoft.txt** | 微软服务 | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Microsoft.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/Microsoft.txt) |
| **Bahamut.txt** | 动画疯 | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Bahamut.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/Bahamut.txt) |
| **BilibiliHMT.txt** | 哔哩哔哩港澳台 | Classical | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/BilibiliHMT.txt) | [Raw](https://raw.githubusercontent.com/Niklaus88/rules/main/rule/BilibiliHMT.txt) |

### 2. 扩展与游戏规则（备用）

| 规则名称 | 业务场景 | CDN 镜像链接 |
| :--- | :--- | :--- |
| **Twitter.txt** | X / Twitter 社交平台 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Twitter.txt) |
| **Adobe.txt** | Adobe 全家桶服务 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Adobe.txt) |
| **Steam.txt** | Steam 客户端与商店 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Steam.txt) |
| **Steam-Download.txt** | Steam 游戏下载 CDN | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Steam-Download.txt) |
| **Steam-Network.txt** | Steam 社区与联机 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/Steam-Network.txt) |
| **SteamCN** | Steam 大陆服直连 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/SteamCN) |
| **youtube-GEOSITE.txt** | YouTube 专用规则 | [jsDelivr](https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/youtube-GEOSITE.txt) |

---

## 替换与使用说明

在 Clash / OpenClash / Egern 的配置文件中，只需将原有的 `xiaolin-007/clash` 链接平滑替换为本仓库链接即可无缝切换：

```yaml
# 原始链接示例：
url: https://fastly.jsdelivr.net/gh/xiaolin-007/clash@main/rule/YouTube.txt

# 替换后的本仓库镜像链接：
url: https://fastly.jsdelivr.net/gh/Niklaus88/rules@main/rule/YouTube.txt
```

---

## 规则特性

- 格式规范：全量保留 Classical YAML / txt 结构，适配 Clash Meta (Mihomo)、Clash Verge Rev、FlClash、OpenClash 及 Egern。
- CDN 加速：默认提供 `fastly.jsdelivr.net` 节点分发，国内网络环境下无需代理即可秒级拉取更新。

---

## 🙏 感谢

- [xiaolin-007 / clash](https://github.com/xiaolin-007/clash)
