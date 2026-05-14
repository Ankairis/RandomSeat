# 随机排座位 / Random Seat Assigner

一个基于 PHP + JavaScript 的随机排座位网页应用。支持自定义座位表、手动取消/选中座位、一键随机分配学号。

A PHP + JavaScript web app for random seat assignment. Customizable grid, click to toggle seats, one-click random student ID assignment.

## 功能 / Features

- 自定义行列数（最大 20×20）
- 点击切换座位选中/取消
- 全选、反选、清除分配
- Fisher-Yates 洗牌算法随机分配学号
- 会话持久化（刷新页面不丢失）
- Material Design 3 风格 UI，支持暗色模式
- 响应式，手机友好

## 快速开始 / Quick Start

### 本地运行（PHP 版）

```bash
php -S localhost:787 -t . random_seat.php
```

打开 `http://localhost:787`。

### 本地运行（纯静态版）

直接双击 `index.html` 或任何静态服务器托管。无需 PHP。

## 部署 / Deploy

### GitHub Pages

1. 仓库 Settings → Pages → Source: **Deploy from branch**
2. Branch: `main`, folder: `/ (root)`
3. Custom domain: 填入 `seat.iriz.top`
4. GitHub 会自动生成 CNAME 文件并配 SSL
5. 以后每次 push 到 main 自动重新部署

DNS 已配好：
- `seat.iriz.top` → `ankairis.github.io` (CF proxied)
- `seat.irix.top` → `ankairis.github.io` (DNS only)

### 验证代码一致性

每次部署显示对应 commit hash，到 GitHub 对比源码即可验证。

## 许可证 / License

MIT
