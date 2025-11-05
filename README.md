# Skymeow

**一个源自 Lolimeow，但视野更开阔、布局更大气的现代 WordPress 主题。**

[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/gpl-2.0) 
[![Requires: WordPress 6.0+](https://img.shields.io/badge/WordPress-6.0%2B-0073aa)](https://wordpress.org/) 
[![PHP: 8.0+](https://img.shields.io/badge/PHP-8.0%2B-777bb3)](https://www.php.net/)

> **Sky** + **meow** = **Skymeow**
>
> 寓意本主题在继承 Lolimeow 简洁基因的同时，致力于为您的网站打造如天空般开阔、通透的视觉体验。它不再局限于传统博客，更能胜任杂志、作品集、个人知识库等多种内容形态。

!screenshot.png

## ✨ 核心特性

Skymeow 在 Lolimeow 的基础上进行了深度优化和重构，主要特色包括：

*   **🎨 开阔的现代设计**：采用更具呼吸感的布局、科学的留白和现代化的视觉元素，让内容本身成为焦点。
*   **📱 全响应式布局**：在手机、平板、桌面设备上均能提供出色的浏览体验。
*   **⚙️ 强大的自定义能力**：通过 WordPress 定制器，轻松修改颜色、字体、布局等，无需触碰代码。
*   **🚀 卓越的性能**：代码简洁高效，遵循 WordPress 最佳实践，确保网站快速加载。
*   **🔍 SEO 友好**：清晰的 HTML 结构和语义化标签，为搜索引擎优化打下良好基础。
*   **📂 多功能模板**：除标准博客布局外，强化或新增了适用于作品集、杂志等模板（如 `portfolio.php`）。

## 📁 文件结构

Skymeow 主题遵循 WordPress 主题标准文件结构，核心模板文件包括：

```
skymeow/
├── assets/           # 静态资源 (CSS, JS, 图片)
├── inc/              # 主题功能扩展文件
├── template-parts/   # 可重用的模板片段
├── functions.php     # 主题核心功能函数 
├── header.php        # 顶部模板 
├── index.php         # 主模板文件 
├── page.php          # 页面模板 
├── single.php        # 文章模板 
├── sidebar.php       # 侧边栏模板 (可选) 
├── footer.php        # 底部模板 
├── style.css         # 主题样式表及元信息 
└── screenshot.png    # 主题预览图 
```

## 🚀 快速安装

### 前提条件

*   一个正常运行的 https://wordpress.org/download/ 环境（建议 6.0 或更高版本）。
*   PHP 7.4 或更高版本。

### 安装方法

1.  **下载主题**：
    *   点击本页右上角的 `Code` -> `Download ZIP` 下载最新压缩包。
    *   或者，使用 Git 克隆：`git clone https://github.com/DearLicy/Skymeow.git`

2.  **上传并激活**：
    *   登录您的 WordPress 后台，进入【外观】->【主题】。
    *   点击【添加新主题】->【上传主题】，选择下载的 `Skymeow.zip` 文件进行安装。
    *   安装成功后，点击【激活】。或者，将解压后的 `skymeow` 文件夹通过 FTP/SFTP 上传到您网站的 `wp-content/themes/` 目录下，然后在后台主题页面激活。

3.  **开始定制**：
    *   激活后，进入 【外观】->【自定义】，开始根据您的喜好调整网站外观。

## ⚙️ 基本使用与定制

### 菜单和微件
激活主题后，建议先到 WordPress 后台的【外观】->【菜单】和【外观】->【微件】区域设置您的导航菜单和侧边栏内容。

### 主题定制器
Skymeow 提供了通过 WordPress 定制器（【外观】->【自定义】）修改外观的选项，例如站点身份（Logo、标题）、颜色、背景图像等。

### 模板层次结构
WordPress 会根据要显示的内容类型自动选择最合适的模板文件。例如，显示单篇文章时会优先使用 `single.php`，如果不存在，则会使用 `index.php`。 Skymeow 遵循此标准。

## 🛠️ 开发

### 模板函数
在主题开发中，会用到许多 WordPress 核心模板函数来动态显示内容，例如：
*   `<?php bloginfo('name'); ?>` - 显示站点标题。
*   `<?php the_title(); ?>` - 显示当前文章/页面标题。
*   `<?php the_content(); ?>` - 显示当前文章/页面主要内容。
*   `<?php if (have_posts()) : while (have_posts()) : the_post(); ?> ... <?php endwhile; endif; ?>` - 主循环，用于遍历并显示文章列表。

### 自定义开发
如果您是开发者并对参与本项目感兴趣，欢迎探索代码。核心功能定义在 `functions.php` 中，模板文件位于根目录及 `template-parts` 文件夹下。

## ❓ 常见问题

**Q: 如何为我的站点创建一个静态首页？**
A: 这是在 WordPress 的【设置】->【阅读】中配置的，与主题无关。Skymeow 完美支持此功能。

**Q: 安装主题后网站布局错乱怎么办？**
A: 请确保您已按照说明正确安装并激活了主题，并检查您的 WordPress 和 PHP 版本是否符合要求。如果问题依旧，请暂时切换回默认主题（如 Twenty Twenty-Four）检查是否是与其他插件冲突。

## 📄 许可证

Skymeow 主题基于 **GNU General Public License v2.0** 发布。这与 WordPress 本身及原主题 Lolimeow 的许可证保持一致。 详情请查看 LICENSE 文件。

## 🙏 致谢

*   感谢 https://github.com/orgs/lolimeow 主题的原作者，为本项目提供了优秀的起点。
*   感谢 WordPress 社区和所有开源开发者。

## 📞 联系与贡献

*   **项目主页与问题反馈**： https://github.com/DearLicy/Skymeow/issues
*   欢迎提交 Pull Request 或提出宝贵的建议！

---

**如果 Skymeow 主题对您有帮助，请给它一个 ⭐ Star！这是对我们最大的鼓励。**
