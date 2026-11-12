# 字间 · iPhone 本地写作网页

这是一个可添加到 iPhone 主屏幕的 PWA 静态网页应用。

## 功能
- 今日写作、字数统计、连续打卡
- 作品档案：查看、编辑、删除
- 自动暂存到当前浏览器本地
- JSON 导入/导出备份
- 总开关：关闭后进入休眠界面，作品数据保留；重新开启即可继续
- Service Worker 离线缓存

## 隐私与数据
作品只保存在当前浏览器的 localStorage，不会自动上传到 GitHub 或其他云端。清除 Safari 网站数据、更换设备等可能导致数据丢失，请定期导出 JSON 备份。若主动复制作品到 ChatGPT 请求点评，文本会发送给 ChatGPT 处理。

## 发布到 GitHub Pages
1. 在 GitHub 新建一个 Public repository，例如 `zijian`。
2. 解压本 ZIP，把其中所有文件（index.html、manifest.webmanifest、sw.js、icon.svg、README.md）上传到仓库根目录。
3. 打开仓库 Settings → Pages。
4. 在 Build and deployment 中选择 `Deploy from a branch`，Branch 选择 `main`、文件夹选择 `/ (root)`，点击 Save。
5. 等待 GitHub Pages 发布完成，网址通常为 `https://你的用户名.github.io/zijian/`。
6. 在 iPhone Safari 打开网址，点分享按钮 → 添加到主屏幕。

提示：PWA 安装和离线缓存需要 HTTPS；GitHub Pages 默认提供 HTTPS。
