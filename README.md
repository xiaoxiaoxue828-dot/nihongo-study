# 旅する日本語 V1.0

独立、免费、无后端的日语旅行学习PWA。采用奶油粉手账风。

## 已实现
- 93天自由学习日历（2026-11-02至2027-02-02）
- Day 1完整课堂（25组平假名/片假名、8个词、自然口语观察、参考资源）
- 随机拼读卡（平假名、片假名、词汇）、错题记录
- 5题配对（平假名→片假名、日语单词→中文）
- 10题自动评分测验
- 学习打卡、学习档案、本地存储、JSON导入导出
- 旅行应急句型、浏览器日语语音合成
- PWA清单与离线静态资源缓存

## 内容边界
Day 2至Day 93课程主题和日期已规划，但具体内容标记为“准备中”。不使用虚构的教材出处。官方教材仅外链，未复制其受版权保护的音频。语音由设备提供，部分iPhone浏览器可能没有可用的日语语音。

## 本地运行
直接打开 index.html 可体验基本功能；要测试PWA，请通过本地HTTP服务器或GitHub Pages打开。

## 部署 GitHub Pages
1. 登录 GitHub，创建公开仓库 `nihongo-study`。
2. 将本文件夹内的 `index.html`、`app.js`、`sw.js`、`manifest.webmanifest`、`icon.svg` 上传至仓库根目录。
3. 仓库 Settings → Pages → Build and deployment → Deploy from a branch，选择 `main` 和 `/(root)`，保存。
4. 等待发布，访问 `https://xiaoxiaoxue828-dot.github.io/nihongo-study/`。
5. 在 iPhone Safari 中打开网址 → 分享 → 添加到主屏幕。

注意：以上网址需在仓库成功创建并发布后才会生效。GitHub Pages 需按 GitHub 当前的公开仓库与账户政策使用。

## 维护
更新课程或前端后应调整 `sw.js` 的 CACHE 常量，避免已安装的PWA继续使用旧缓存。学习数据保存在浏览器localStorage，清理站点数据可能导致记录丢失，请定期导出JSON。
