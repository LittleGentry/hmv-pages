# HotfixMiniVerify 支持页

本仓库用于托管 App Store 提审所需的两个必填页面：

- `privacy-policy.html` — 隐私政策 URL
- `support.html` — 支持 URL

## 部署到 GitHub Pages

```bash
cd store/pages
git init
git add -A
git commit -m "Add privacy policy and support pages"
git branch -M main
git remote add origin https://github.com/<你的用户名>/hmv-pages.git
git push -u origin main
```

推送后在 GitHub 仓库页面：**Settings ▸ Pages**，Source 选 `Deploy from a branch`，Branch 选 `main` + `/ (root)`，保存。

等 1 到 2 分钟，页面地址为：

```
https://<你的用户名>.github.io/hmv-pages/privacy-policy.html
https://<你的用户名>.github.io/hmv-pages/support.html
```

## 填进 App Store Connect

在 App Store 标签下的「App 信息」和「版本信息」里填入上面两个地址。

## 验证

用无痕窗口打开两个链接，确认能正常显示。Apple 审核时会真的访问这两个地址，填之前务必先自己验证一次。
