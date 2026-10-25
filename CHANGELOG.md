# Changelog

このプロジェクトの主な変更点を記録します。

書式は [Keep a Changelog](https://keepachangelog.com/ja/1.1.0/) に、バージョンの付け方は [Semantic Versioning](https://semver.org/lang/ja/) に従います。

## [Unreleased]

### Added

- CSS変数で速度と色を変更できるようにしました。
  - `--gaming-duration`：1周の時間（初期値 `5s`）
  - `--gaming-color-1`〜`--gaming-color-3`：アニメーションの色（初期値 `magenta` / `yellow` / `cyan`）
- OSで「動きを減らす」設定（`prefers-reduced-motion: reduce`）をしている環境では、アニメーションしないようにしました。クラス指定だけでなく、`animation` プロパティにアニメーション名を自分で指定した場合も止まります。
- サンプルページ（`index.html`）を追加しました。
- ライセンスファイル（`LICENSE`）を追加しました。

### Changed

- `gaming-filter` の色相が一定の速さで回るようにしました。これまでは区間ごとに速さがわずかにずれていました。
- `package.json` の `homepage` をサンプルページ（GitHub Pages）のURLに変更しました。

### Fixed

- `gaming-border-block-end-color` クラスがアニメーションしない不具合を修正しました。キーフレーム名が `gaming-block-end-color` と誤っていました。

### Docs

- READMEに、JavaScript・CSS・CDNから読み込む方法を追記しました。
- READMEの例を、CSS変数 `--gaming-duration` が効く書き方に修正しました。

## [1.0.2] - 2023-11-16

### Added

- `gaming-fill`（SVGの塗りの色）を追加しました。

## [1.0.1] - 2023-07-02

### Added

- `gaming-filter`（画像の色相を回転）を追加しました。
- 次のクラスを追加しました。
  - `gaming-outline-color`
  - `gaming-text-decoration-color`
  - `gaming-border-inline-start-color`
  - `gaming-border-inline-end-color`
  - `gaming-border-block-start-color`
  - `gaming-border-block-end-color`（キーフレーム名の誤りにより、このバージョンでは動作しません）

## [1.0.0] - 2023-06-24

### Added

- 初回リリース。次のクラスを提供します。
  - `gaming-color`
  - `gaming-background-color`
  - `gaming-border-color`
  - `gaming-border-top-color`
  - `gaming-border-right-color`
  - `gaming-border-bottom-color`
  - `gaming-border-left-color`

[Unreleased]: https://github.com/ishi720/gaming-css/compare/1.0.2...HEAD
[1.0.2]: https://github.com/ishi720/gaming-css/compare/1.0.1...1.0.2
[1.0.1]: https://github.com/ishi720/gaming-css/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/ishi720/gaming-css/releases/tag/1.0.0
