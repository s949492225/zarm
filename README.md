<p align="center">
  <a href="http://zarm.design">
    <img width="200" src="https://zarm.design/images/logo.732d9561.svg">
  </a>
</p>

<h1 align="center">Zarm</h1>

<div align="center">

  [![Build Status](https://www.travis-ci.org/ZhongAnTech/zarm.svg?branch=dev)](https://www.travis-ci.org/ZhongAnTech/zarm)
  [![Coverage Status](https://img.shields.io/coveralls/ZhongAnTech/zarm/dev.svg)](https://coveralls.io/github/ZhongAnTech/zarm?branch=dev)
  ![JS gzip size](https://img.badgesize.io/https://unpkg.com/zarm@beta/dist/zarm.min.js?compression=gzip&label=gzip%20size:%20JS)
  ![CSS gzip size](https://img.badgesize.io/https://unpkg.com/zarm@beta/dist/zarm.min.css?compression=gzip&label=gzip%20size:%20CSS)
  [![NPM downloads](https://img.shields.io/npm/dm/zarm.svg)](https://npmjs.org/package/zarm) 
  [![dependencies Status](https://david-dm.org/ZhongAnTech/zarm/status.svg)](https://david-dm.org/ZhongAnTech/zarm)
  [![peerDependencies Status](https://david-dm.org/ZhongAnTech/zarm/peer-status.svg)](https://david-dm.org/ZhongAnTech/zarm?type=peer)
  [![devDependencies Status](https://david-dm.org/ZhongAnTech/zarm/dev-status.svg)](https://david-dm.org/ZhongAnTech/zarm?type=dev)
  [![Netlify Status](https://api.netlify.com/api/v1/badges/7afc45a9-dcac-4475-9903-d3896bc200ed/deploy-status)](https://app.netlify.com/sites/zarm/deploys)
  [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FZhongAnTech%2Fzarm.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FZhongAnTech%2Fzarm?ref=badge_shield)
  [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ZhongAnTech/zarm?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

  众安科技基于 React、React-Native 研发的一款适用于企业级的移动端UI组件库。
</div>

Zarm 的命名，灵感来源于众安保险秉承的理念：做有温度的保险。Zarm = za + warm，za代表“众安”，warm有“温暖”的含义，以重合的a字母为中心，各取左右两部分。追求极致的用户体验，致力于做有温度的组件库也是zarm项目发起的初衷。

## 版本

- 稳定版：[![npm package](https://img.shields.io/npm/v/zarm.svg)](https://www.npmjs.org/package/zarm)
- 开发版：[![npm package](https://img.shields.io/npm/v/zarm/beta.svg)](https://www.npmjs.org/package/zarm)

## 浏览器支持

- ios
- Android 4.0+

## 安装

### 使用 npm 或 yarn 安装（推荐）

```bash
# npm
npm install zarm@beta --save

# yarn
yarn add zarm@beta
```

### 或者通过 link 和 script 标签分别引入样式文件和js脚本文件（不推荐）

```html
<link rel="stylesheet" href="https://unpkg.com/zarm@beta/dist/zarm.min.css">
<script type="text/javascript" src="https://unpkg.com/zarm@beta/dist/zarm.min.js"></script>
```

## 使用

### 全组件引入

```js
import { Button, Cell } from 'zarm';
import 'zarm/dist/zarm.min.css';
```

### 按需加载

> 注意：zarm 默认支持基于 ES module 的 tree shaking，不使用以下插件也会有按需加载的效果。

- 使用 [babel-plugin-import](https://github.com/ant-design/babel-plugin-import) 自动加载Sass文件（推荐）

```js
  // .babelrc or babel-loader option
  {
    "plugins": [
      ['import', {
        libraryName: 'zarm',
        style: true, // or 'css'
      }],
    ]
  }
```

```js
import { Button, Cell } from 'zarm';
```

- 手动引入

```js
import Button from 'zarm/lib/button'; // 加载js
import 'zarm/lib/button/style/css'; // 加载css
// import 'zarm/lib/button/style'; // 加载scss
```

### 定制主题

通过修改css变量定义达到定制主题的效果

```js
document.documentElement.style.setProperty('--theme-primary', '#108ee9');
```

变量名可参考 [default.scss](https://github.com/ZhongAnTech/zarm/blob/dev/components/style/themes/default.scss)

## 社区

| issue | gitter | 微信群 |
| :--- | :--- | :--- |
| [github issue](https://github.com/ZhongAnTech/zarm/issues) | [ZhonganTech/zarm](https://gitter.im/ZhonganTech/zarm) | <img src="https://user-images.githubusercontent.com/9812721/69521400-d3708100-0f99-11ea-9669-2cea28ec66f7.png" width="60" /> |

## 开源协议

MIT

[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FZhongAnTech%2Fzarm.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2FZhongAnTech%2Fzarm?ref=badge_large)