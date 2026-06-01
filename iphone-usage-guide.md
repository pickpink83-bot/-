# iPhone 使用方式

## 推荐方式：添加到主屏幕

1. 把 `outputs` 里的这几个文件放到一个 HTTPS 静态网站：
   - `personal-password-vault.html`
   - `manifest.json`
   - `service-worker.js`
   - `vault-icon.svg`
2. 在 iPhone 上用 Safari 打开这个网页地址。
3. 点分享按钮，选择“添加到主屏幕”。
4. 之后从主屏幕打开“密码库”即可。

数据会保存在 iPhone 当前这个网页 App 的本地存储里。主密码不会上传或保存。

## 可选方式：做成真正的 iOS App

可以用 SwiftUI + Keychain + 本地数据库做原生 App，但需要 Apple 开发者账号、Xcode、真机签名。如果只是个人使用，PWA 更轻、更快，也不需要上架。

## 安全提醒

- 一定要记住主密码，忘记后无法恢复。
- 建议定期点“导出加密备份”，把备份文件保存到 iCloud Drive 或电脑。
- 不建议把网页托管在会注入广告脚本的平台。
