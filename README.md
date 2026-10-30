# Neutrilizer

NEUTRINO を歌声エンジンとして使う、**非公式**の VST3 歌声プラグインです（Windows 64bit）。
DAW の楽器トラックに挿して、ノート・歌詞・ピッチ・タイミングを編集し、DAW の再生に合わせて歌わせます。

> 本ソフトウェアは STUDIO NEUTRINO および調声支援ツールの作者とは無関係の非公式ツールです。
> NEUTRINO 本体と歌声ライブラリは同梱していません。

## ダウンロード

**[最新版のダウンロード（Releases）](https://github.com/wassawasa/Neutrilizer/releases/latest)** から `Neutrilizer-<版>-win64.zip` を取得してください。

※ このページの緑の「Code」ボタンからダウンロードできるのはこの説明だけで、ソフトウェア本体は入っていません。

## 必要なもの

- Windows 10 / 11（64bit）。Windows 10 では [Microsoft Edge WebView2 ランタイム](https://developer.microsoft.com/microsoft-edge/webview2/) が必要です
- [NEUTRINO](https://studio-neutrino.com/) 標準版（Tau v3.2 以降）と歌声ライブラリ
- VST3 に対応した DAW（Reaper で動作を確認しています）

## インストール

1. DAW を終了し、zip を展開します
2. 中の `Neutrilizer.vst3` フォルダを、中身ごと `C:\Program Files\Common Files\VST3` にコピーします（管理者の許可を求められます）
3. DAW でプラグインを再スキャンし、楽器トラックに **Neutrilizer** を挿します
4. 初回はプラグインの設定画面で、NEUTRINO 標準版のフォルダを指定します

`Neutrilizer.vst3` の中には、歌声を作るエンジンも入っています。フォルダの中身は分けずにコピーしてください。

- **更新:** DAW を終了して 30 秒ほど待ってから、新しい `Neutrilizer.vst3` で上書きします
- **削除:** DAW を終了して `Neutrilizer.vst3` を消します

詳しくは zip に同梱の README.txt を参照してください。

## 主な機能

- ピアノロールでのノート・歌詞の編集、楽譜の読み込み（MusicXML / MIDI / UST）
- ピッチ編集（ペン・直線・なめらか筆・消しゴム・範囲の加工）、ノートごとのビブラート
- 音素タイミングの編集、ブレス・語頭ブレス
- Reaper では、テンポと拍子を Reaper から受け取り、ノートと歌詞を MIDI アイテムとして同期

## 利用上の注意

- 本ソフトウェアは無保証です。使用によって生じたいかなる損害についても、作者は責任を負いません
- NEUTRINO と各歌声ライブラリは、それぞれの利用規約に従って使用してください。生成した音声の利用も同様です
- 第三者のソフトウェアのライセンス表記は、`Neutrilizer.vst3` の中の `Contents\Resources\THIRD-PARTY-NOTICES.txt` にあります
- VST is a registered trademark of Steinberg Media Technologies GmbH.
