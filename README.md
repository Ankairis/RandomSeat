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

```bash
# 启动 PHP 内置服务器
php -S localhost:787 -t . random_seat.php
```

打开 `http://localhost:787` 即可使用。

## 依赖 / Requirements

- PHP 8.0+（仅用于会话持久化和页面路由）

## 许可证 / License

MIT
