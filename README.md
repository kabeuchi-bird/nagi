# nagi

薙刀式配列を[kanata](https://github.com/jtroo/kanata)でエミュレートします。kanataは高機能なキーボードリマッパです。

Linuxの自環境（Cachyos, KDE Plasma （wayland）, fcitx5-mozc）上で動かした場合に、unicodeを直接IMEに送ると変換等ができないためフォークしました。

キーマップ内容の変更は以下2つです。

- macro機能を用いてキーに対応するローマ字を送るように変更
- kanata起動時にqwerty配列(=リマップ前の配列そのまま)を読み込むようにし、半角／全角キー押下で薙刀式とqwerty配列を切り替える方式とした
- 編集モードの実装

カスタマイズしたい場合は、上記リンクからマニュアルをご参照ください。

## 薙刀式バージョン

v17 ベスト版

## 使い方

1. nagi.kbdと[kanata](https://github.com/jtroo/kanata)をダウンロード
1. kanataのショートカットを作成し、リンク先に`-c nagi.kbd`と追加
1. ショートカットから起動

![リンク先を変更](shortcut.png)
