# Xing的博客 - superYXing.github.io

[![Hexo Version](https://img.shields.io/badge/Hexo-7.3.0-blue.svg)](https://hexo.io/)
[![Theme](https://img.shields.io/badge/Theme-Matery-brightgreen.svg)](https://github.com/blinkfox/hexo-theme-matery)

这是基于 Hexo 静态博客框架构建的个人博客网站，使用了 Matery 主题。

## 📋 项目简介

这是一个已经生成并部署的 Hexo 静态博客站点，包含完整的静态资源文件。

- **博客地址**: [yongxing.codes](https://yongxing.codes)
- **生成器**: Hexo 7.3.0
- **主题**: hexo-theme-matery
- **部署平台**: GitHub Pages

## 📁 项目结构

```
superYXing.github.io/
├── 2024/                      # 博客文章（按年月日组织）
│   └── 09/                    # 2024年9月的文章
│       ├── 08/                # 9月8日的文章
│       ├── 17/                # 9月17日的文章
│       ├── 18/                # 9月18日的文章
│       ├── 20/                # 9月20日的文章
│       ├── 22/                # 9月22日的文章
│       ├── 25/                # 9月25日的文章
│       └── 30/                # 9月30日的文章
├── about/                     # 关于页面
├── archives/                  # 归档页面
├── categories/                # 分类页面
│   └── Markdown/              # Markdown分类
├── contact/                   # 联系页面
├── image/                     # 图片页面
├── musics/                    # 音乐页面
├── page/                      # 分页页面
├── tags/                      # 标签页面
│   └── Markdown/              # Markdown标签
├── css/                       # 自定义样式文件
│   ├── barrager.css          # 弹幕样式
│   ├── dark.css              # 深色模式
│   ├── gallery.css           # 相册样式
│   ├── matery.css            # 主题主样式
│   └── ...
├── js/                        # 自定义JavaScript文件
│   ├── matery.js             # 主题核心JS
│   ├── search.js             # 搜索功能
│   └── ...
├── libs/                      # 第三方库文件
│   ├── jquery/               # jQuery库
│   ├── materialize/          # Materialize UI框架
│   ├── aos/                  # 滚动动画库
│   ├── fancybox/             # 图片灯箱
│   ├── prism/                # 代码高亮
│   ├── typed/                # 打字机效果
│   ├── gitalk/               # Gitalk评论系统
│   ├── valine/               # Valine评论系统
│   ├── twikoo/               # Twikoo评论系统
│   └── ...
├── medias/                    # 媒体资源
│   ├── banner/               # 横幅图片
│   ├── barrager/             # 弹幕资源
│   ├── featureimages/        # 特色图片
│   ├── images/               # 其他图片
│   └── reward/               # 打赏图片
├── images/                    # 图片资源
├── index.html                 # 首页
├── 404.html                   # 404错误页面
├── search.xml                 # 搜索索引文件
└── cname                      # 自定义域名配置
```

## ✨ 功能特性

- 📱 响应式设计，完美适配移动端
- 🎨 Material Design 风格
- 🌙 深色模式支持
- 🔍 本地搜索功能
- 🏷️ 标签和分类系统
- 📊 文章归档
- 💬 多种评论系统支持（Gitalk、Valine、Twikoo）
- 🖼️ 相册展示功能
- 🎵 音乐播放器
- 💰 打赏功能
- 📈 访问统计（不蒜子）
- 🎬 多种背景特效（樱花、雪花、星空等）
- 🎯 代码高亮（Prism.js）
- 📝 Markdown 支持
- 🎭 打字机效果
- 🚀 页面加载动画（AOS）

## 🔧 如何继续使用

### 方式一：作为已部署的静态站点（推荐用于快速浏览）

如果这是已经部署到 GitHub Pages 的静态文件，您可以：

1. **直接访问网站**: 访问 [yongxing.codes](https://yongxing.codes) 或 [superYXing.github.io](https://superYXing.github.io)

2. **本地预览**:
   ```bash
   # 使用 Python 启动简单的 HTTP 服务器
   python -m http.server 8000
   
   # 或使用 Node.js 的 http-server
   npx http-server -p 8000
   
   # 然后访问 http://localhost:8000
   ```

### 方式二：恢复 Hexo 源码继续开发（推荐用于继续写作）

**⚠️ 注意**: 当前目录只包含生成的静态文件，没有 Hexo 源码。如果您想继续写博客，需要：

1. **找到 Hexo 源码目录**
   
   通常 Hexo 项目结构如下：
   ```
   blog-source/              # Hexo 源码目录（需要找到这个）
   ├── _config.yml          # Hexo 配置文件
   ├── package.json         # 依赖配置
   ├── source/              # 源文件目录
   │   ├── _posts/         # 文章Markdown源文件
   │   ├── about/          # 关于页面源文件
   │   └── ...
   ├── themes/              # 主题目录
   │   └── matery/         # Matery主题
   ├── node_modules/        # 依赖包
   └── public/              # 生成的静态文件（就是当前目录）
   ```

2. **如果有源码，在源码目录执行**:
   ```bash
   # 安装依赖
   npm install
   
   # 创建新文章
   hexo new "文章标题"
   
   # 本地预览
   hexo server
   # 访问 http://localhost:4000
   
   # 生成静态文件
   hexo generate
   # 或简写
   hexo g
   
   # 部署到 GitHub Pages
   hexo deploy
   # 或简写
   hexo d
   
   # 清理缓存
   hexo clean
   ```

3. **如果源码丢失，需要重建项目**:
   ```bash
   # 安装 Hexo CLI
   npm install -g hexo-cli
   
   # 初始化新项目
   hexo init blog-source
   cd blog-source
   npm install
   
   # 安装 Matery 主题
   git clone https://github.com/blinkfox/hexo-theme-matery.git themes/matery
   
   # 修改 _config.yml 中的 theme 配置
   # theme: matery
   
   # 配置主题（参考 Matery 主题文档）
   # https://github.com/blinkfox/hexo-theme-matery/blob/develop/README_CN.md
   ```

### 方式三：部署到其他平台

您可以将这些静态文件部署到：

- **GitHub Pages** (当前方式)
- **Vercel**: 直接导入 GitHub 仓库
- **Netlify**: 拖拽部署或连接 Git
- **云服务器**: 上传到 Nginx/Apache 的 web 目录
- **CDN**: 配合对象存储使用

## 📝 写作流程（如果有源码）

1. **创建新文章**:
   ```bash
   hexo new "我的新文章"
   ```

2. **编辑文章**:
   - 在 `source/_posts/` 目录下找到对应的 `.md` 文件
   - 使用 Markdown 编辑器编写内容

3. **本地预览**:
   ```bash
   hexo server
   ```

4. **生成并部署**:
   ```bash
   hexo clean && hexo generate && hexo deploy
   ```

## 🎨 主题配置

Matery 主题支持丰富的配置选项：

- **首页轮播图**
- **个人信息卡片**
- **社交媒体链接**
- **友情链接**
- **背景特效**
- **评论系统**
- **访问统计**
- **音乐播放器**
- **相册功能**

详细配置请参考：[Matery 主题文档](https://github.com/blinkfox/hexo-theme-matery/blob/develop/README_CN.md)

## 📦 依赖的主要库

- **jQuery 3.6.0** - JavaScript 库
- **Materialize CSS** - Material Design UI 框架
- **AOS** - 滚动动画库
- **Prism.js** - 代码语法高亮
- **FancyBox** - 图片灯箱效果
- **Typed.js** - 打字机效果
- **Gitalk/Valine/Twikoo** - 评论系统
- **APlayer/MetingJS** - 音乐播放器
- **不蒜子** - 访问统计

## 🔍 常见问题

### Q: 如何修改博客内容？
A: 需要找到 Hexo 源码目录，修改 `source/_posts/` 下的 Markdown 文件，然后重新生成静态文件。

### Q: 如何更换主题？
A: 在 Hexo 源码目录中安装新主题，修改 `_config.yml` 中的 `theme` 配置。

### Q: 如何添加新页面？
A: 使用 `hexo new page "页面名称"` 命令创建新页面。

### Q: 如何自定义域名？
A: 修改 `cname` 文件中的域名，并在域名服务商处配置 DNS 解析。

### Q: 网站加载慢怎么办？
A: 可以考虑使用 CDN 加速静态资源，或将图片压缩优化。

## 📄 许可证

本项目遵循相应开源许可证。

- Hexo: [MIT License](https://github.com/hexojs/hexo/blob/master/LICENSE)
- Matery Theme: [Apache License 2.0](https://github.com/blinkfox/hexo-theme-matery/blob/develop/LICENSE)

## 📞 联系方式

- 博客: [yongxing.codes](https://yongxing.codes)
- GitHub: [superYXing](https://github.com/superYXing)

## 🎯 下一步建议

1. **备份源码**: 确保 Hexo 源码已经备份到 Git 仓库
2. **分离管理**: 建议使用两个分支
   - `source` 分支：存放 Hexo 源码
   - `main/master` 分支：存放生成的静态文件
3. **自动化部署**: 配置 GitHub Actions 实现自动构建和部署
4. **定期备份**: 定期备份文章和配置文件

---

⭐ 如果觉得这个博客不错，欢迎 Star 支持！
