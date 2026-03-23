# L的个人主页

这是一个用于展示个人信息的大学生个人主页，适合发布在GitHub Pages上。

## 页面特点

- 响应式设计，适配各种屏幕尺寸
- 现代化UI风格，渐变色背景
- 包含所有核心必备信息
- 易于修改和扩展

## 页面内容

### 核心必备信息
- 基础身份标识（姓名、头像、标签）
- 校园背景（学校、学院、专业、学制、学历）
- 专业技能（技术类、非技术类）
- 核心课程
- 联系方式

## 如何部署到GitHub Pages

### 1. 创建GitHub仓库

1. 登录你的GitHub账号
2. 点击右上角的 "+" 图标，选择 "New repository"
3. 仓库名称建议使用：`your-username.github.io`（替换为你的GitHub用户名）
4. 选择 "Public" 或 "Private"（Public可以免费使用GitHub Pages）
5. 点击 "Create repository"

### 2. 上传文件到GitHub

你可以通过以下两种方式之一上传文件：

#### 方式一：通过GitHub网页界面上传

1. 在新创建的仓库页面，点击 "uploading an existing file"
2. 将 `index.html` 文件拖拽到上传区域
3. 点击 "Commit changes"

#### 方式二：通过Git命令上传（推荐）

在本地终端中执行以下命令：

```bash
# 初始化Git仓库
git init

# 添加文件
git add index.html README.md

# 提交更改
git commit -m "Initial commit - personal homepage"

# 关联远程仓库（替换为你的仓库地址）
git remote add origin https://github.com/your-username/your-repo-name.git

# 推送到GitHub
git branch -M main
git push -u origin main
```

### 3. 启用GitHub Pages

1. 进入你的GitHub仓库页面
2. 点击 "Settings" 选项卡
3. 在左侧菜单中找到 "Pages"（通常在 "Code and automation" 部分）
4. 在 "Build and deployment" 部分：
   - Source 选择 "Deploy from a branch"
   - Branch 选择 "main"（或 "master"）
   - 文件夹选择 "/ (root)"
5. 点击 "Save"

### 4. 访问你的个人主页

等待几分钟后，你的个人主页就可以通过以下地址访问了：

```
https://your-username.github.io/
```

（替换 `your-username` 为你的GitHub用户名）

## 如何自定义

### 修改个人信息

编辑 `index.html` 文件，找到相应的部分进行修改：

- 姓名和头像：修改 `.header` 部分
- 校园背景：修改校园背景 section
- 专业技能：修改专业技能 section
- 核心课程：修改核心课程 section
- 联系方式：修改联系我 section

### 修改颜色主题

在 `index.html` 的 `<style>` 标签中，找到以下渐变色并修改：

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### 添加头像

1. 将你的头像图片命名为 `avatar.jpg` 或 `avatar.png`
2. 将图片文件放在与 `index.html` 同一目录下
3. 修改 `index.html` 中的头像部分：

```html
<div class="avatar">
    <img src="avatar.jpg" alt="头像" style="width: 100%; height: 100%; border-radius: 50%; object-fit: cover;">
</div>
```

## 文件结构

```
.
├── index.html    # 主页面文件
└── README.md     # 说明文档
```

## 技术栈

- HTML5
- CSS3
- 原生JavaScript（无需额外框架）

## 许可证

MIT License - 你可以自由使用和修改这个页面。
