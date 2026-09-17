# 个人学术主页

纯静态网站（HTML + CSS），无需构建，可直接部署到 GitHub Pages。

## 文件
- `index.html` — 全部内容，按 `<!-- ==== 区块 ==== -->` 注释分段
- `style.css` — 样式（自动适配深色模式和手机）
- `assets/` — 头像、CV.pdf 等

## 部署到 GitHub Pages
1. 在 GitHub 新建仓库，名字必须是 `<你的用户名>.github.io`
2. 上传本文件夹所有文件：
   ```bash
   git init && git add . && git commit -m "init homepage"
   git branch -M main
   git remote add origin https://github.com/<用户名>/<用户名>.github.io.git
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source 选 `main` 分支 `/ (root)`
4. 一两分钟后访问 `https://<用户名>.github.io`

## 常见修改
- 换头像：把照片放到 `assets/avatar.jpg`，改 `index.html` 里的 `avatar.svg`
- 加论文：复制 Publications 里的一个 `<li class="pub">` 块
- 放 CV：把 PDF 命名为 `assets/CV.pdf`
