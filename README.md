# 高校「情報Ⅰ」デジタル化教材

高校「情報Ⅰ」の授業で使える、**音声のデジタル化**と**画像のデジタル化**を体験的に学ぶための Web 教材です。  
すべて **単体 HTML ファイル** で構成され、外部ライブラリなし・通信なしで動作します。

## 構成ファイル

```text
.
├─ audio_digitization_oscilloscope.html
├─ image_digitization_simulator.html
├─ teacher_screen_digitalization_github.html(index.html)
├─ student_screen_digitalization_github.html
└─ README.md
```

## 各ファイルの役割

### `audio_digitization_oscilloscope.html`
音声のデジタル化教材です。

主な機能:
- オシロスコープ表示
- FFT（周波数スペクトル）表示
- 標本化周波数の変更
- 量子化ビット数の変更
- マイク入力
- 録音・再生
- エイリアシング観察
- データ量計算

### `image_digitization_simulator.html`
画像のデジタル化教材です。

主な機能:
- 元画像とデジタル化後画像の比較表示
- 解像度変更
- 階調ビット数変更
- RGB / グレースケール / 白黒2値 切り替え
- 画素値の確認
- カメラ入力・画像ファイル読み込み
- データ量計算

### `teacher_screen_digitalization_github.html`
先生用画面です。

主な機能:
- 音教材 / 画像教材の切り替え
- 授業進行メモ表示
- 生徒用画面との連携
- プレビュー表示

### `student_screen_digitalization_github.html`
生徒用画面です。

主な機能:
- 音教材 / 画像教材の切り替え
- シンプルな提示用画面
- 先生用画面との同期（同一ブラウザ内）

## 使い方

### 1. 単独で使う場合
- `audio_digitization_oscilloscope.html` を開くと、音の教材が使えます。
- `image_digitization_simulator.html` を開くと、画像の教材が使えます。

### 2. 先生用 / 生徒用の 2 画面で使う場合
1. `teacher_screen_digitalization_github.html` を開きます。
2. 先生用画面のボタンから生徒用画面を開くか、`student_screen_digitalization_github.html` を別ウィンドウで開きます。
3. 同じブラウザ内で開いている場合、教材切り替えが自動で同期します。

## 動作環境

推奨ブラウザ:
- Google Chrome
- Microsoft Edge
- Safari
- Firefox

いずれも最新版を推奨します。

## 利用上の注意

### マイク・カメラ使用について
- **マイク**や**カメラ**を使う場合は、通常 **HTTPS 環境** が必要です。
- ローカルファイルとして開く場合は、ブラウザ設定によって利用できることがあります。
- 学校サーバーや LMS に配置する場合は、**HTTPS 配信**を推奨します。

### プライバシー
- 外部通信は行いません。
- 音声・画像データは端末内で処理されます。
- カメラ利用時は肖像権・プライバシーへの配慮を行ってください。

## GitHub Pages での公開

この教材は相対パスで構成されているため、同じディレクトリに配置すれば GitHub Pages でも公開できます。

例:
- `https://あなたのユーザー名.github.io/リポジトリ名/teacher_screen_digitalization_github.html`
- `https://あなたのユーザー名.github.io/リポジトリ名/student_screen_digitalization_github.html`

## 授業での活用例

### 音のデジタル化
- 標本化周波数を下げて波形の変化を観察する
- ビット数を下げて量子化雑音を確認する
- FFT で周波数成分を確認する
- エイリアシングを視覚的・聴覚的に確認する

### 画像のデジタル化
- 解像度を下げてモザイク化を確認する
- 階調ビット数を下げてトーンジャンプを確認する
- 画素値と2進数表現の対応を確認する
- データ量と画質の関係を考察する

## ライセンス

授業内での利用・複製・改変・配布は自由です。  
必要に応じて学校や授業の実態に合わせて調整してください。

## 作成メモ

- 単体 HTML
- 外部 CDN 不使用
- オフライン利用可能
- 教材としてそのまま配布可能
