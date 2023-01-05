<div align='center'>
<h1>BlockCV</h1>
<img src='README.assets/logo.png' alt='BlockCV - online resume editor' width='344'/>
</div>

<p align='center'>
BlockCV is an online resume editor that allows users to easily create and customize professional resumes. 
The application uses Editor.js as the core editor, which is a block-style editor for rich media stories. It outputs clean data in JSON format, and is designed to be API extendable and pluggable.
</p>

<div align='center'>
<b>English</b> | <a href="README.zh-CN.md">简体中文</a>
</div>

## Features

- ⚡  [Vue 3](https://github.com/vuejs/vue-next), [Vite 2](https://github.com/vitejs/vite), [pnpm](https://pnpm.js.org/) - born with fastness
- 💪 [Typescript](https://www.typescriptlang.org/) - of course! necessary
- 💡 [Editor.js](https://github.com/codex-team/editor.js) -  block-style editor for rich media stories. It outputs clean data in JSON format
- 📦 API pluggable for easy extension and customization
- 📥 Drag and drop interface for adding and rearranging resume blocks
- 🤙🏻 Resume auto-formatting
- 🎉 Export as PDF
- 🌼 Live preview of resume design
- 📜 Multiple resume templates to choose from
- 🌍 [I18n ready](./src/locales)

### Coding Style

- [@kirklin/eslint-config](https://github.com/kirklin/eslint-config)

### Recommended IDE Setup

- [VSCode](https://code.visualstudio.com/)
- [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar)


## Try it now!

### Clone to local

```bash
git clone https://github.com/kirklin/BlockCV.git
cd BlockCV
pnpm i
```

## Usage

### Development

Just run and visit http://localhost:8888

```bash
pnpm run dev
```

### Build

To build the App, run

```bash
pnpm run build
```

And you will see the generated file in `dist` that ready to be served.


### Deploy on Netlify

Go to [Netlify](https://app.netlify.com/start) and select your clone, `OK` along the way, and your App will be live in a minute.

### Docker Production Build

First, build the BlockCV image by opening the terminal in the project's root directory.

```bash
docker buildx build . -t viteboot:latest
```

Run the image and specify port mapping with the `-p` flag.

```bash
docker run --rm -it -p 8080:80 viteboot:latest
```

