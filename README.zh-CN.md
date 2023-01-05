<div align='center'>
<h1>BlockCV</h1>
<img src='README.assets/logo.png' alt='BlockCV - 在线简历编辑器' width='344'/>
</div>

<p align='center'>
BlockCV是一款在线简历编辑器，使用户可以轻松创建和自定义专业简历。
该应用使用Editor.js作为编辑器核心，它是一款专门用于创建富文本的块式编辑器。它以JSON格式输出数据，并且可以轻松扩展和插入API。
</p>

<div align='center'>
<a href="README.md">English</a> | <b>简体中文</b>
</div>

## 特性

- ⚡  [Vue 3](https://github.com/vuejs/vue-next), [Vite](https://github.com/vitejs/vite), [pnpm](https://pnpm.js.org/) - 为速度而生
- 💪 [Typescript](https://www.typescriptlang.org/) - 强大的类型检查
- 💡 [Editor.js](https://github.com/codex-team/editor.js) - 富文本的块式编辑器。它以JSON格式输出数据
- 📦 易于扩展和自定义的API插件
- 📥 可拖拽组件，方便添加和重新排列简历块
- 🤙🏻 简历自动排版
- 🎉 可导出为PDF
- 🌼 实时预览简历
- 📜 多种简历模板可供选择
- 🌍 [I18n 国际化](./src/locales)

### 编码风格

- [@kirklin/eslint-config](https://github.com/kirklin/eslint-config)

### 推荐的 IDE 设置

- [VSCode](https://code.visualstudio.com/)
- [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar)


## 快来试试吧！！

### 克隆到本地

```bash
git clone https://github.com/kirklin/BlockCV.git
cd BlockCV
pnpm i
```

## 使用

### 开发

只需要执行以下命令就可以在 http://localhost:8888 中看到

```bash
pnpm run dev
```

### 构建

构建该应用只需要执行以下命令

```bash
pnpm run build
```

然后你会看到用于发布的 `dist` 文件夹被生成。


### 部署到 Netlify

前往 [Netlify](https://app.netlify.com/start) 并选择你的仓库, 一路 `OK` 下去，稍等一下后，你的应用将被创建.

### Docker Production Build

首先，在项目的根目录下打开终端，构建BlockCV镜像。

```bash
docker buildx build . -t viteboot:latest
```

运行镜像，用 "-p" 指定端口映射。

```bash
docker run --rm -it -p 8080:80 viteboot:latest
```

