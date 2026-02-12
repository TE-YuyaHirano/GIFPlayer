# GIFPlayer

GIF をキャンバス描画で再生・停止できるシンプルなプレイヤーです。長押しで別画像（PNG/JPG）を表示できます。

**主な機能**
- GIF 再生/停止（フレーム位置を保持）
- 長押し 5 秒で静止画に切り替え（離すと再生に戻る）
- ローディング表示（オーバーレイ）
- URL パラメータで GIF/速度/静止画を指定

**ファイル構成**
- `index.html`
- `asset/slotmachine.gif`
- `asset/last.png`（長押しで表示する画像。任意）

**使い方**
ブラウザで `index.html` を開くだけです。

**URL パラメータ**
- `gif` 再生する GIF のパスや URL
- `speed` 再生速度（数値）
- `alt` 長押しで表示する画像のパスや URL（PNG/JPG）

**例**
- `index.html`（`asset/slotmachine.gif` を再生）
- `index.html?gif=asset/slotmachine.gif&speed=50`
- `index.html?gif=asset/slotmachine.gif&alt=asset/last.png`
- `index.html?gif=https://example.com/sample.gif&alt=https://example.com/last.jpg`

**操作**
- 赤いボタンをタップで再生/停止
- 赤いボタンを 5 秒長押しで静止画表示、離すと GIF に戻る

**注意点**
- 大きい GIF は iOS で落ちる場合があります。解像度やファイルサイズを軽くすると安定します。
- `speed` を極端に大きくすると負荷が上がります。

