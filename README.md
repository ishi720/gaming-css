# Overview

`gaming-css`は、ゲーミングなスタイリングするCSSです

# Badge

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/f813675d8bd0407e8b06c8a531e00666)](https://app.codacy.com/gh/ishi720/gaming-css/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![npm version](https://badge.fury.io/js/gaming-css.svg)](https://badge.fury.io/js/gaming-css)
![npm version](https://img.shields.io/npm/dt/gaming-css.svg)

# Install

npm

```
npm i gaming-css
```
yarn 

```
yarn add gaming-css
```

# Import

JavaScript（webpack や Vite など）

```js
import 'gaming-css/gaming.css';
```

CSS

```css
@import 'gaming-css/gaming.css';
```

CDN（インストール不要）

```html
<!-- jsDelivr -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/gaming-css@1/gaming.css">

<!-- unpkg -->
<link rel="stylesheet" href="https://unpkg.com/gaming-css@1/gaming.css">
```

# Usage

htmlの`class属性`やcssの`animation-name`としてパラメータに指定できます。

パラメータ名は、以下の既存プロパティ名に対応しています。

| 既存プロパティ名 | パラメータ名 |
| - | - |
| color | gaming-color |
| background-color | gaming-background-color |
| border-color | gaming-border-color |
| border-top-color | gaming-border-top-color |
| border-right-color | gaming-border-right-color |
| border-bottom-color | gaming-border-bottom-color |
| border-left-color | gaming-border-left-color |
| outline-color | gaming-outline-color |
| text-decoration-color | gaming-text-decoration-color |
| border-inline-start-color | gaming-border-inline-start-color |
| border-inline-end-color | gaming-border-inline-end-color |
| border-block-start-color | gaming-border-block-start-color |
| border-block-end-color | gaming-border-block-end-color |
| filter | gaming-filter |
| fill | gaming-fill |

### htmlの`class属性`に指定する

```html
<div class="gaming-background-color">背景色</div>
```

### 複数のアニメーションするようにカスタマイズする

```css
div {
	animation: gaming-color 5s linear infinite,
	           gaming-border-color 5s linear infinite;
}
```

### hoverなどの疑似クラスに適用したい場合

```css
a:hover {
    animation: gaming-background-color 5s linear infinite;
}
```

### 速度や色を変更したい場合

CSS変数で上書きできます。`gaming-filter`は速度のみ変更できます。

| CSS変数 | 内容 | 初期値 |
| - | - | - |
| --gaming-duration | 1周の時間 | 5s |
| --gaming-color-1 | 1色目 | Magenta |
| --gaming-color-2 | 2色目 | yellow |
| --gaming-color-3 | 3色目 | Cyan |

```css
.gaming-color {
    --gaming-duration: 2s;
    --gaming-color-1: red;
    --gaming-color-2: lime;
    --gaming-color-3: blue;
}
```
