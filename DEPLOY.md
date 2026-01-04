# 部署指南 / Deployment Guide

## 本地 Git 仓库已准备就绪！

所有文件已经提交到本地 Git 仓库。现在您需要：

## 步骤 1: 在 GitHub 上创建新仓库

1. 访问 https://github.com/new
2. 仓库名称填写：`my-resume` (或您喜欢的其他名称)
3. **不要**勾选 "Initialize this repository with a README" (我们已经有了)
4. 点击 "Create repository"

## 步骤 2: 连接本地仓库到 GitHub

在终端中运行以下命令（将 `YOUR_USERNAME` 替换为您的 GitHub 用户名）：

```bash
cd /Users/huiyuezhou/Documents/Projects/my-resume
git remote add origin https://github.com/YOUR_USERNAME/my-resume.git
git push -u origin main
```

或者，如果您使用 SSH（推荐）：

```bash
git remote add origin git@github.com:YOUR_USERNAME/my-resume.git
git push -u origin main
```

## 步骤 3: 启用 GitHub Pages

1. 在 GitHub 仓库页面，点击 **Settings**（设置）
2. 在左侧菜单中找到 **Pages**
3. 在 "Source" 部分：
   - 选择 "Deploy from a branch"
   - Branch 选择：`main`
   - Folder 选择：`/ (root)`
4. 点击 **Save**

## 步骤 4: 访问您的网站

几分钟后，您的网站将可以通过以下地址访问：

```
https://YOUR_USERNAME.github.io/my-resume/
```

---

## 如果需要更新网站

修改文件后，运行：

```bash
git add .
git commit -m "更新说明"
git push
```

GitHub Pages 会自动重新部署您的网站。

