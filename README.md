# 孙蒙鸽个人简历网站

一个现代化的学术个人简历网站，展示您在科学计量学、知识图谱与智能情报领域的研究成果和学术成就。

## 🌟 特性

- **响应式设计** - 完美适配桌面、平板和手机
- **现代化UI** - 使用渐变色彩和阴影效果
- **平滑动画** - 滚动动画和悬停效果
- **交互功能** - 表单验证、通知系统
- **性能优化** - 防抖滚动、懒加载
- **无障碍支持** - 键盘导航、屏幕阅读器友好

## 📁 文件结构

```
github_cv/
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # JavaScript功能
├── README.md           # 项目说明
└── 孙蒙鸽简历(复制).pdf  # 原始简历文件
```

## 👨‍🎓 个人简介

- **姓名**: 孙蒙鸽
- **学历**: 中国科学院大学 信息管理专业 博士研究生
- **研究方向**: 科学计量学、知识图谱与智能情报
- **学术成果**: 累计发表CSSCI/SCI论文18篇，总被引168次
- **参与项目**: 17项科研项目
- **荣誉奖项**: 博士研究生国家奖学金、情报科学创新团队奖等

## 🚀 快速开始

1. **直接打开**
   ```bash
   # 在浏览器中打开 index.html
   open index.html
   ```

2. **本地服务器**（推荐）
   ```bash
   # 使用Python
   python -m http.server 8000
   
   # 使用Node.js
   npx serve .
   
   # 使用PHP
   php -S localhost:8000
   ```

3. **访问网站**
   - 打开浏览器访问 `http://localhost:8000`

## 🎨 自定义指南

### 修改个人信息

在 `index.html` 中修改以下内容：

```html
<!-- 修改姓名 -->
<h1 class="hero-title">你好，我是 <span class="highlight">您的姓名</span></h1>

<!-- 修改职位描述 -->
<p class="hero-subtitle">您的职位 | 技能标签 | 个人标签</p>

<!-- 修改个人介绍 -->
<p class="hero-description">
    您的个人介绍和职业目标
</p>
```

### 修改技能

在 `index.html` 的技能部分：

```html
<div class="skill-item">
    <span>技能名称</span>
    <div class="skill-bar">
        <div class="skill-progress" style="width: 85%"></div>
    </div>
</div>
```

### 修改项目

在 `index.html` 的项目部分：

```html
<div class="project-card">
    <div class="project-image">
        <i class="fas fa-项目图标"></i>
    </div>
    <div class="project-content">
        <h3>项目名称</h3>
        <p>项目描述</p>
        <div class="project-tech">
            <span>技术栈1</span>
            <span>技术栈2</span>
        </div>
        <div class="project-links">
            <a href="项目链接" class="btn btn-small">查看演示</a>
            <a href="源码链接" class="btn btn-small btn-outline">源代码</a>
        </div>
    </div>
</div>
```

### 修改联系信息

在 `index.html` 的联系部分：

```html
<div class="contact-item">
    <i class="fas fa-envelope"></i>
    <div>
        <h3>邮箱</h3>
        <p>your.email@example.com</p>
    </div>
</div>
```

### 修改颜色主题

在 `styles.css` 的 `:root` 部分：

```css
:root {
    --primary-color: #6366f1;    /* 主色调 */
    --secondary-color: #8b5cf6;  /* 次要色调 */
    --accent-color: #06b6d4;     /* 强调色 */
    /* 其他颜色变量... */
}
```

## 📱 响应式断点

- **桌面**: > 768px
- **平板**: 768px - 480px
- **手机**: < 480px

## 🎯 功能说明

### 导航功能
- 固定导航栏，滚动时背景模糊
- 移动端汉堡菜单
- 平滑滚动到对应部分

### 动画效果
- 页面加载时的淡入动画
- 滚动时的元素出现动画
- 技能进度条动画
- 悬停效果和涟漪效果

### 表单功能
- 联系表单验证
- 实时错误提示
- 成功提交通知

### 性能优化
- 滚动事件防抖
- 图片懒加载
- CSS动画硬件加速

## 🔧 技术栈

- **HTML5** - 语义化标签
- **CSS3** - 现代布局和动画
- **JavaScript ES6+** - 交互功能
- **Font Awesome** - 图标库
- **Google Fonts** - 字体

## 📋 浏览器支持

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 🚀 部署到GitHub Pages

1. **创建GitHub仓库**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/yourusername/your-repo.git
   git push -u origin main
   ```

2. **启用GitHub Pages**
   - 进入仓库设置
   - 找到 "Pages" 选项
   - 选择 "main" 分支
   - 保存设置

3. **访问网站**
   - 网站将在 `https://yourusername.github.io/your-repo` 上线

## 📞 联系信息

如需帮助或建议，请联系：
- 邮箱: sunmengge@example.com
- GitHub: [您的GitHub链接]

## 📄 许可证

MIT License - 可自由使用和修改

---

**注意**: 请根据您的实际情况修改个人信息、项目内容和联系方式。 