# データ直行カメラ（パイロット版）

スマホのブラウザで紙を撮り、そのまま自分の Google ドライブへ送る Web アプリ。
スマホ本体には写真を残さない。

- 公開URL: https://gjm8.github.io/data-chokko-camera/
- 本体: `index.html` 1枚（ビルドの道具・外部サーバーなし）
- ログイン: Google Identity Services のトークン方式／スコープは `drive.file` のみ
- 送り先: マイドライブ/データ直行カメラ/{未整理, 自治会, 光熱費, ノート}（初回にアプリが作る）
- ファイル名: `YYYY-MM-DD_HHMMSS.jpg`（日本時間・シャッターを押した時刻）

仕様書・設定の控え・セッションログは Google ドライブの
`claude_home_pc\projects\データ直行カメラapp\` にある。

## 開発の続け方（どの PC でも）

```
git clone https://github.com/gjm8/data-chokko-camera.git
```

`index.html` を直して push すると、1〜2分で公開URLに反映される。
`CONFIG.VERSION` を上げておくと、スマホで新しい版が読み込まれたかを画面右下で確かめられる。
