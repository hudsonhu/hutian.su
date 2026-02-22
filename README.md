# Tiansu's Blog（Hexo）

这是一个基于 [Hexo](https://hexo.io/) 搭建的个人博客项目，当前站点配置如下：

- 站点标题：`Tiansu's Blog`
- 站点地址：`https://blog.tiansu.hu`
- 语言：`zh-CN`
- 主题：`hueman`（本地主题目录：`themes/hueman`）

## 环境要求

- Node.js：`20.x`
- npm：`10.x`

项目中的版本约束见 `package.json` 的 `engines` 字段。

## 快速开始

1. 安装依赖

```bash
npm install
```

2. 本地启动开发服务器

```bash
npm run server
```

默认访问地址通常为 `http://localhost:4000`。

3. 生成静态文件

```bash
npm run build
```

生成结果位于 `public/` 目录。

4. 清理缓存和生成产物

```bash
npm run clean
```

## 常用内容维护

1. 新建文章

```bash
npx hexo new post "文章标题"
```

2. 新建草稿

```bash
npx hexo new draft "草稿标题"
```

3. 发布草稿（转为正式文章）

```bash
npx hexo publish "草稿标题"
```

文章默认放在 `source/_posts/`，并使用 front-matter 管理标题、日期、标签、分类等信息。

## 项目结构

```text
.
├── _config.yml             # Hexo 主配置
├── package.json            # 依赖与脚本命令
├── scaffolds/              # 新建文章/页面模板
├── source/
│   ├── _posts/             # 博客文章
│   ├── about/              # 关于页面
│   └── images/             # 站点图片资源
└── themes/
    └── hueman/             # 当前启用主题
```

## 部署说明

仓库已预留 `npm run deploy` 命令（`hexo deploy`），如需使用请先在 `_config.yml` 中补充 `deploy` 配置，并安装对应部署插件（例如 `hexo-deployer-git`）。

## 参考文档

- Hexo 官方文档：https://hexo.io/docs/
- Hexo 配置说明：https://hexo.io/docs/configuration.html
