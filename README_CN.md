# CLI Proxy API Plus 管理中心

本仓库是基于 `router-for-me/main` 管理面板的 fork。

本 README 只描述相对 `router-for-me/main` 不一样的新增或保留模块。

[English](README.md)

## 本 fork 新增或保留的模块

### Kiro 配额

新增 **Kiro** 凭据的配额展示能力：

- 展示 Kiro 订阅与基础额度信息。
- 展示免费试用状态。
- 当后端返回时展示凭据暂停状态。

### GitHub Copilot 配额

新增 **GitHub Copilot** 凭据的配额展示能力：

- 展示 Copilot 套餐信息。
- 展示聊天、补全和高级交互额度。
- 支持展示后端返回的不限量额度。

### Ampcode 提供商集成

保留 `router-for-me/main` 已移除的 **Ampcode** provider 模块：

- 保留 AI Providers workbench 中的 Ampcode provider 注册。
- 保留 Ampcode 上游地址与上游 API key 配置。
- 保留 upstream API key 映射配置。
- 保留模型映射配置与强制映射开关。
- 保留 Ampcode Management API client 与相关类型定义。

### 使用统计 iframe

新增基于 **iframe** 实现的 **使用统计** 模块：

- 配置 `usage-statistics-url` 后，侧边栏会显示使用统计入口。
- iframe 地址应填写 https://github.com/Willxup/cpa-usage-keeper 这个项目部署后的访问地址。
- 可在可视化配置面板的远程管理中填写该部署地址，也可直接在 `config.yaml` 中配置 `usage-statistics-url`。

## 上游参考

通用使用方式、开发命令、配置与未改动功能说明，请参考上游项目文档：

- `router-for-me/main`: https://github.com/router-for-me/Cli-Proxy-API-Management-Center
- CLI Proxy API: https://github.com/router-for-me/CLIProxyAPI
