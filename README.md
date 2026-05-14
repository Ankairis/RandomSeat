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

### Cloudflare Pages

Fork 此仓库，在 CF Pages 关联 GitHub 仓库：

1. CF Dashboard → Pages → Create a project → Connect to GitHub
2. 选择 `Ankairis/RandomSeat`
3. Build command: `sed -i "s/__GIT_HASH__/$(git rev-parse HEAD)/" index.html`
4. Build output: `.`
5. 部署完成后页面底部显示当前 commit hash

也可用 GitHub Actions（`.github/workflows/deploy.yml`），需在仓库设置添加 `CF_API_TOKEN` secret。

### 验证代码一致性

每次部署显示对应 commit hash，到 GitHub 对比源码即可验证。

## 许可证 / License

MIT
