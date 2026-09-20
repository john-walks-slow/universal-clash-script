# 通用 Clash 配置

简单易用的 Clash 配置，基于 proxy-providers 自动融合多个机场的节点信息，根据个人使用经验持续优化。

## 特性

- 根据节点名称按地区分类，创建对应的 `url-test` 组。使用时只需选择地区即可获得最优连接。
- 强大、实用的策略组，PROXY 出口支持在首选和次选地区间自动 fallback；DEFAULT 组用于选择未命中流量的处理方式。
- 简洁、优化的分流策略和 DNS 配置，能应对大多数情况。
- 易于自定义的黑白名单和地区分流策略。

## 使用

适用于 FlClash / Clash Verge Rev 等 Mihomo 系客户端。

1. 导入配置文件：[universal_clash_profile](https://github.com/john-walks-slow/universal-clash-script/raw/refs/heads/main/universal_clash_profile.yaml)
2. 在 `proxy-providers` 部分填入机场订阅
3. 在 `rule-providers` 部分可以自定义黑白名单和路由规则
4. 开始上网吧！

### 通过脚本重载使用（已废弃，不推荐）

在已有配置的 `重载-脚本` 中启用脚本：[universal_clash_script](https://github.com/john-walks-slow/universal-clash-script/raw/refs/heads/main/universal_clash_script.js)

## FAQ

#### 直接使用机场配置可以连通，使用本配置无法连通？

机场可能配置了特殊的 hosts 规则。请检查机场配置中是否有 hosts: 部分，粘贴到我们的配置中即可。

## 许可证

MIT
