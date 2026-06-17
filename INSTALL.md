# iPhone 安装说明

这个版本已经升级成 PWA，可以像简易 App 一样添加到 iPhone 主屏幕。

## 最推荐的安装方式

1. 把整个文件夹上传到一个 HTTPS 网站，例如 GitHub Pages、Netlify、Vercel 或 Cloudflare Pages。
2. 用 iPhone Safari 打开网站地址。
3. 点击 Safari 底部的分享按钮。
4. 选择“添加到主屏幕”。
5. 名称保留“请假管理”或自行修改，然后点“添加”。
6. 回到 iPhone 桌面，点击新图标打开。

## 本地测试方式

1. 电脑和 iPhone 连接同一个 Wi-Fi。
2. 在这个文件夹启动本地网页服务。
3. iPhone Safari 打开电脑的局域网地址，例如：

```text
http://192.168.1.23:8080/index.html
```

4. 可以用 Safari 的“添加到主屏幕”测试图标和页面效果。

本地 HTTP 地址通常不能稳定启用离线缓存；正式使用建议放到 HTTPS 网站。

## 已包含的 PWA 文件

- `manifest.webmanifest`：App 名称、图标、启动方式。
- `service-worker.js`：离线缓存。
- `assets/icons/`：iPhone 和 PWA 图标。
- `index.html`：主页面。

## 注意

这不是 App Store 安装包，不需要 Apple 开发者账号。它是可添加到主屏幕的网页 App，适合当前这种简易移动端工具。
