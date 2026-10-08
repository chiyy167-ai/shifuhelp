# 保利管道 · 师傅上门（三端演示 PWA）

把原有单页 HTML 演示封装为可在 **Android / iOS** 主屏幕打开的 Progressive Web App。

## 在线演示

部署到 GitHub Pages 后访问仓库 Pages 地址（见下方）。

## 本地预览

PWA / Service Worker 需要通过 HTTP(S) 访问（不要用 `file://`）：

```bash
npx --yes serve .
```

浏览器打开提示的本地地址即可。

## 手机安装（演示）

### Android（Chrome）

1. 用 Chrome 打开站点
2. 菜单 → **安装应用** / **添加到主屏幕**
3. 从主屏幕图标以独立窗口打开

### iOS（Safari）

1. 用 Safari 打开站点
2. 分享 → **添加到主屏幕**
3. 从主屏幕图标打开（standalone）

> iOS 对 PWA 支持有限：可全屏、可缓存；推送等能力受限。本项目为前端演示，无后端。

## 结构

| 文件 | 说明 |
|------|------|
| `index.html` | 三端演示主页面 |
| `manifest.webmanifest` | Web App Manifest |
| `sw.js` | Service Worker（离线缓存） |
| `icons/` | 应用图标 |

## 说明

- 演示数据均为虚构，仅用于产品流程展示。
- 客户端 / 水工端 / 管理端在同一页面顶部切换。
