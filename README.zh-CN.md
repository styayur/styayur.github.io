# styayur — 旧 URL 兼容入口

[English](README.md) · [当前主站](https://styayur.co.uk)

本仓库是保留旧 GitHub Pages URL 的最小重定向入口，不是独立维护的作品集，也不是生产主站源码。

## 路由

| 入口 | 目标 | 机制 |
| --- | --- | --- |
| [根目录](https://styayur.github.io/)及 `/index.html` | [styayur.co.uk](https://styayur.co.uk) | JavaScript 保留 query/fragment；`/index.html` 归一为 `/` |
| `/projects/`、`/writing/` 等旧路径 | [styayur.co.uk](https://styayur.co.uk) 上的同一路径 | 最小 `404.html` 浏览器回退保留路径、query 和 fragment |
| [`/calligraphy-studio/`](https://styayur.github.io/calligraphy-studio/) | [Calligra 演示](https://styayur.github.io/calligra/) | 兼容页面跳转时保留 query/hash |

其他项目的 Pages 部署独立于根入口；仓库更名本身不会保留项目 Pages 地址。只要这些 URL 仍由此 Pages 部署提供，就保持仓库可用且不归档。替代机制实际验证前不要删除。

目标 origin 固定，URL 参数不能选择其他主机。Pages 会先以 HTTP 404
提供旧路径回退页，再由脚本跳到新页。关闭 JavaScript 时，静态刷新和链接
只去主站首页；动态保留路径、query、fragment 需要 JavaScript。主站上原本
不存在的路径仍可能返回 404。现有 Calligra 兼容页仍优先服务其项目 URL。

## 维护与验证

只修改对应重定向入口，并检查目标、备用链接、HTTPS 和实际部署。保留旧路径，在部署后测试 query/fragment；旧日期的观测不能代替新检查。

公开的[历史引擎](https://github.com/styayur/digital-garden-engine)保留渲染器来源与许可，已经归档，不构建当前主站。[GitHub Profile](https://github.com/styayur)是公开账号入口。

## 许可与反馈

保留现有 [LICENSE](LICENSE) 和历史声明。通过 [Issues](https://github.com/styayur/styayur.github.io/issues) 报告可复现的错误跳转，提供不含敏感信息的完整 URL。不在兼容仓库中增加网站功能、作品集数据或框架。
