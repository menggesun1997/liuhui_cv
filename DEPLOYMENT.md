# GitHub Pages 部署指南

## 🚀 快速部署到GitHub Pages

### 方法一：使用GitHub Desktop（推荐新手）

1. **下载GitHub Desktop**
   - 访问 https://desktop.github.com/
   - 下载并安装GitHub Desktop

2. **创建新仓库**
   - 打开GitHub Desktop
   - 点击 "File" → "New Repository"
   - 填写仓库信息：
     - Name: `sunmengge-cv` 或 `personal-website`
     - Description: `孙蒙鸽个人简历网站`
     - 选择 "Public"
     - 勾选 "Initialize this repository with a README"

3. **上传文件**
   - 将项目文件夹拖拽到GitHub Desktop
   - 或者点击 "Add" → "Add Existing Repository"
   - 选择您的项目文件夹

4. **提交并推送**
   - 在GitHub Desktop中填写提交信息
   - 点击 "Commit to main"
   - 点击 "Push origin"

5. **启用GitHub Pages**
   - 在GitHub网页上打开您的仓库
   - 点击 "Settings" 标签
   - 滚动到 "Pages" 部分
   - Source选择 "Deploy from a branch"
   - Branch选择 "main"
   - 点击 "Save"

6. **访问网站**
   - 等待几分钟后，您的网站将在以下地址上线：
   - `https://您的用户名.github.io/仓库名`

### 方法二：使用命令行

1. **初始化Git仓库**
   ```bash
   cd /Users/sunmengge/Downloads/github_cv
   git init
   ```

2. **添加文件**
   ```bash
   git add .
   git commit -m "Initial commit: 个人简历网站"
   ```

3. **创建GitHub仓库**
   - 访问 https://github.com/new
   - 创建新仓库，不要初始化README

4. **连接并推送**
   ```bash
   git remote add origin https://github.com/您的用户名/仓库名.git
   git branch -M main
   git push -u origin main
   ```

5. **启用GitHub Pages**
   - 在GitHub仓库页面点击 "Settings"
   - 找到 "Pages" 选项
   - Source选择 "Deploy from a branch"
   - Branch选择 "main"
   - 保存设置

### 方法三：使用GitHub CLI

1. **安装GitHub CLI**
   ```bash
   # macOS
   brew install gh
   
   # 登录
   gh auth login
   ```

2. **创建仓库并推送**
   ```bash
   gh repo create sunmengge-cv --public --source=. --remote=origin --push
   ```

3. **启用Pages**
   ```bash
   gh repo edit --enable-pages
   ```

## 📝 自定义域名（可选）

如果您有自己的域名，可以设置自定义域名：

1. **在GitHub仓库设置中**
   - 进入 "Settings" → "Pages"
   - 在 "Custom domain" 中输入您的域名
   - 点击 "Save"

2. **在域名提供商处**
   - 添加CNAME记录指向 `您的用户名.github.io`

## 🔧 更新网站

每次修改代码后，需要重新推送：

```bash
git add .
git commit -m "更新网站内容"
git push
```

GitHub Pages会自动重新部署您的网站。

## 📊 查看访问统计

1. 在GitHub仓库页面点击 "Insights"
2. 选择 "Traffic" 查看访问统计

## 🎨 自定义建议

### 添加个人照片
1. 将照片文件放在项目根目录
2. 在HTML中引用：
   ```html
   <img src="your-photo.jpg" alt="孙蒙鸽" class="profile-photo">
   ```

### 添加Google Analytics
1. 注册Google Analytics
2. 获取跟踪代码
3. 在HTML的`<head>`部分添加跟踪代码

### 添加SEO优化
1. 在HTML中添加meta标签
2. 创建sitemap.xml
3. 添加结构化数据

## 🚨 注意事项

1. **文件大小限制**: GitHub Pages有文件大小限制
2. **构建时间**: 首次部署可能需要几分钟
3. **HTTPS**: GitHub Pages自动提供HTTPS
4. **缓存**: 浏览器可能会缓存旧版本，强制刷新即可

## 📞 常见问题

### Q: 网站显示404错误
A: 检查仓库设置中的Pages配置是否正确

### Q: 样式没有加载
A: 确保CSS文件路径正确，检查文件名大小写

### Q: 图片不显示
A: 检查图片路径，确保图片文件已上传

### Q: 网站更新后没有变化
A: 清除浏览器缓存，或等待几分钟让GitHub重新部署

---

**部署完成后，您的个人简历网站就可以通过 `https://您的用户名.github.io/仓库名` 访问了！** 🎉 