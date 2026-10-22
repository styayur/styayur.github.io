# styayur — 旧 URL 兼容入口

[English](README.md) · [当前主站](https://styayur.co.uk)

本仓库是保留旧 GitHub Pages URL 的最小重定向入口，不是独立维护的作品集，也不是生产主站源码。

## 路由

| 入口 | 目标 | 机制 |
| --- | --- | --- |
| [根目录](https://styayur.github.io/)及 `/index.html` | [styayur.co.uk](https://styayur.co.uk) | 保留 HTML 跳转、canonical 与可读备用链接 |
| [`/calligraphy-studio/`](https://styayur.github.io/calligraphy-studio/) | [Calligra 演示](https://styayur.github.io/calligra/) | 兼容页面跳转时保留 query/hash |

其他项目的 Pages 部署独立于根入口；仓库更名本身不会保留项目 Pages 地址。只要这些 URL 仍由此 Pages 部署提供，就保持仓库可用且不归档。替代机制实际验证前不要删除。

## 维护与验证

只修改对应重定向入口，并检查目标、备用链接、HTTPS 和实际部署。保留旧路径，在部署后测试 query/fragment；旧日期的观测不能代替新检查。

公开的[历史引擎](https://github.com/styayur/digital-garden-engine)保留渲染器来源与许可，已经归档，不构建当前主站。[GitHub Profile](https://github.com/styayur)是公开账号入口。

## 许可与反馈

保留现有 [LICENSE](LICENSE) 和历史声明。通过 [Issues](https://github.com/styayur/styayur.github.io/issues) 报告可复现的错误跳转，提供不含敏感信息的完整 URL。不在兼容仓库中增加网站功能、作品集数据或框架。
