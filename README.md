# Markdown Editor — A full-featured WYSIWYG editor for markdown
# Markdown Editor — フル機能のWYSIWYG Markdownエディター

[![badge_title](https://vsmarketplacebadges.dev/version-short/zaaack.markdown-editor.png)](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor) [![](https://vsmarketplacebadges.dev/installs-short/zaaack.markdown-editor.png)](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor) [![](https://vsmarketplacebadges.dev/rating-short/zaaack.markdown-editor.png)](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor)

## Demo / デモ

![demo](./demo.gif)

## Additional Features / 追加機能

### Custom CSS Unification / カスタムCSSの一本化 (v0.0.2)
- **EN**: Removed the `markdown-editor.customCss` setting. Custom CSS is now automatically loaded only from `media/default-custom.css` within the extension for a unified and simple design.
- **JA**: `markdown-editor.customCss` 設定を廃止しました。デザインと管理をシンプルにするため、拡張機能内の `media/default-custom.css` からのみ自動的にCSSを読み込む仕様に一本化しました。

### Single Scrollbar & Light Theme / 一重スクロールバー化とテーマのLight固定 (v0.0.2)
- **EN**: Fixed the Vditor theme to `Light` and completely removed the double scrollbars on the webview for a cleaner layout.
- **JA**: Vditorのテーマを `Light` に強制固定し、Webview上の二重スクロールバーを完全に排除してレイアウトを最適化しました。

## Features / 主な機能

1. What You See Is What You Get (WYSIWYG)
   - 見たまま編集できるWYSIWYG（ウィジウィグ）形式
2. Auto sync changes between the VSCode editor and webview
   - VSCodeエディターとWebview間の自動同期
3. Copy markdown/html
   - Markdown/HTMLとしてのコピー
4. Uploaded/pasted/drag-dropped images will be auto-saved to the `assets` folder
   - アップロード/ペースト/ドラッグ＆ドロップされた画像を `assets` フォルダへ自動保存
5. Multi-theme support
   - 複数テーマのサポート
6. Shortcut keys
   - ショートカットキー対応
7. Multiple editing modes: instant Rendering mode (**Recommand!**) / WYSIWYG mode / split screen mode
   - 複数の編集モード: Instant Renderingモード（**推奨!**）/ WYSIWYGモード / 分割画面モード
8. Markdown extensions
   - Markdown拡張構文のサポート
9. Multiple graph support including KaTeX / Mermaid / Graphviz / ECharts / abc.js(notatioan) / ...
   - KaTeX / Mermaid / Graphviz / ECharts / abc.js 等を含む多数のグラフ・数式対応
10. For more usage please see [vditor](https://github.com/Vanessa219/vditor)
    - 詳細な使い方は [vditor](https://github.com/Vanessa219/vditor) を参照してください。

## Install / インストール

[https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor)

## Supported syntax / 対応シンタックス

[demo article](https://ld246.com/guide/markdown)
[デモ記事はこちら](https://ld246.com/guide/markdown)

## Usage / 使い方

### 1. Command mode in markdown file / コマンドパレットからの起動

- open a markdown file
  - Markdownファイルを開く
- type `cmd-shift-p` to enter command mode
  - `cmd-shift-p` を押してコマンドパレットを開く
- type `markdown-editor: Open with markdown editor`
  - `markdown-editor: Open with markdown editor` と入力して選択

### 2. Key bindings / キーバインディング

- open a markdown file
  - Markdownファイルを開く
- type `ctrl+shift+alt+m` for win or `cmd+shift+alt+m` for mac
  - Windowsの場合は `ctrl+shift+alt+m`、Macの場合は `cmd+shift+alt+m` を押下

### 3. Explorer Context menu / エクスプローラーのコンテキストメニュー

- right click on markdown file
  - エクスプローラー上でMarkdownファイルを右クリック
- then click `Open with markdown editor`
  - `Open with markdown editor` をクリック

### 4. Editor title context menu / エディタタブのコンテキストメニュー

- right click on a opened markdown file's tab title
  - 開いているMarkdownファイルの上部タブを右クリック
- then click `Open with markdown editor`
  - `Open with markdown editor` をクリック

### 5. Open With... and Set Default Editor / デフォルトエディターの設定

- right click on a markdown file in Explorer
  - エクスプローラーでMarkdownファイルを右クリック
- click `Open With...`
  - `Open With...`（アプリケーションから開く）をクリック
- select `Markdown Editor` to open temporary
  - 一時的に開く場合は `Markdown Editor` を選択
- or click `Configure default editor...` and select `Markdown Editor` to set it as default
  - デフォルトに設定する場合は `Configure default editor...` をクリックし、`Markdown Editor` を選択

### Custom CSS (custom layout and vditor personalization) / カスタムCSSについて

Edit your settings.json and add
`settings.json` を編集して以下を追加します：

```
"markdown-editor.customCss": "my custom css rules"

// Eg: "markdown-editor.customCss": ".vditor-ir pre.vditor-reset {line-height: 32px;padding-right: calc(100% - 800px) !important; margin-left: 100px;    font-family: system-ui !important;}"
```

## Acknowledgement / 謝辞

- [vscode](https://github.com/microsoft/vscode)
- [vditor](https://github.com/Vanessa219/vditor)

## Todo / 今後の予定

- [ ] Using [Custom Text Editor](https://code.visualstudio.com/api/extension-guides/custom-editors#custom-text-editor) ([demo](https://github.com/gera2ld/markmap-vscode))

## License / ライセンス

MIT

## Support / サポート

If you like this extension make sure to star the repo. I am always looking for new ideas and feedback. In addition, it is possible to [donate via paypal](https://www.paypal.me/zaaack).
もしこの拡張機能を気に入っていただけたら、リポジトリにスターをお願いします。常に新しいアイデアやフィードバックをお待ちしています。また、[PayPal経由での寄付](https://www.paypal.me/zaaack)も可能です。
