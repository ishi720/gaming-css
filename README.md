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

### htmlの`class属性`に指定する

```html
<div class="gaming-background-color">背景色<div>
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
