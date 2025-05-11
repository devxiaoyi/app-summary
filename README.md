# App 技术支持与隐私政策网站

用于 App Store 的技术支持网址、隐私政策网址，可部署到 GitHub Pages 上。

## 网站内容

- **技术支持页面**：提供联系方式和常见问题解答
- **隐私政策页面**：详细的隐私政策声明，符合 App Store 要求

## GitHub Pages 部署步骤

1. 在 GitHub 上创建新仓库（例如 `app-support-site`）

2. 初始化本地 Git 仓库并提交文件：

```bash
git init
git add .
git commit -m "初始提交：技术支持和隐私政策网站"
```

3. 添加远程 GitHub 仓库并推送：

```bash
git remote add origin https://github.com/您的用户名/app-support-site.git
git branch -M main
git push -u origin main
```

4. 在 GitHub 仓库设置中启用 GitHub Pages：
   - 进入仓库 → Settings → Pages
   - Source 选择 "main" 分支
   - 保存设置

5. 几分钟后，您的网站将在以下网址可用：
   `https://您的用户名.github.io/app-support-site/`

## 在 App Store Connect 中使用

1. 登录 [App Store Connect](https://appstoreconnect.apple.com/)
2. 导航至您的应用 → App 信息
3. 在 "支持 URL" 字段中输入您的技术支持页面 URL
   例如：`https://您的用户名.github.io/app-support-site/`
4. 在 "隐私政策 URL" 字段中输入您的隐私政策页面 URL
   例如：`https://您的用户名.github.io/app-support-site/privacy.html`
5. 保存更改

## 本地预览

您可以使用任何静态文件服务器在本地预览网站：

```bash
python -m http.server 8000
```

然后在浏览器中访问 `http://localhost:8000`