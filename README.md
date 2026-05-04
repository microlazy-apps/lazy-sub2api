# lazy-sub2api

[懒猫微服](https://lazycat.cloud) 上的 [sub2api](https://github.com/Wei-Shaw/sub2api) 一键部署 ——
AI API 网关平台，把 Claude / OpenAI / Gemini 等订阅统一聚合成可分发的 API 配额。

## 安装

下载最新 lpk：[Releases](https://github.com/microlazy-apps/lazy-sub2api/releases/latest)

```sh
lpk-manager install ./cloud.lazycat.app.sub2api-*.lpk
```

或在懒猫应用商店搜索「Sub2API」直接安装。

## 使用

装好后访问 `https://sub2api.{你的微服域名}` 看 Web 界面。

首次安装时会要求设置：
- **管理员邮箱** — 登录用户名
- **管理员密码** — 至少 8 位

登录后在「账户管理」里添加上游 AI 服务（OAuth / API Key），再到「API 密钥」生成派发给用户的 key 即可。

## 开发

仓库结构：sub2api 上游以 git subtree 形式存放在 `vendor/sub2api/`。
详细开发说明（发布流程、镜像复制、模板渲染）见 [CLAUDE.md](CLAUDE.md)。

## License

LGPL-3.0，沿用上游 [Wei-Shaw/sub2api](https://github.com/Wei-Shaw/sub2api) 协议。
见 [LICENSE](LICENSE)。
