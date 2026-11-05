# 小影视 (XTV)

基于 **FongMi/TV** 二次开发的聚合播放器，支持 Android TV、手机、平板，支持本地文件与 URL 播放。

- **下载**：[👉 Releases 最新安装包](https://github.com/xiaohh9527/XTV/releases/tag/latest)
- **上游**：https://github.com/FongMi/TV
- **许可证**：GPL-3.0

## 主要功能

- **浏览**：分类筛选、跨站搜索、收藏、播放记录与无痕模式。
- **播放**：倍速、字幕、弹幕、片段跳过、画中画与后台播放。
- **直播**：分组选台、节目表、频道收藏与线路切换。
- **操作**：电视遥控器、手机手势、DLNA 投放与接收。
- **互通**：网页遥控、文件传输、记录同步与 Android Auto。

## 云端构建

本仓库使用 GitHub Actions 自动化构建（`.github/workflows/build.yml`，JDK 21 + Gradle 直编）。

每次推送到 `main` 分支后，会自动：

1. 编译 **Leanback（电视端）+ Mobile（手机端）**、**arm64_v8a + armeabi_v7a** 四个 Debug APK；
2. 发布到 Releases 的 `latest` 标签下，可直接下载安装。

爬虫开发（Java / Python / QuickJS）说明见 [CatVodSpider](https://github.com/FongMi/CatVodSpider)。
