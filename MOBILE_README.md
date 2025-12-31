# とさでん交通在線モニター - スマホ版

## 📱 スマホ専用 12列表示版

### ファイル一覧

**新規アップロードするファイル:**
1. `mobile.html` - スマホ専用HTMLファイル
2. `mobile.js` - スマホ専用JavaScriptファイル

**既存のファイル（そのまま使用）:**
- `data/stops.txt`
- `data/stop_times.txt`
- `data/unyo_平日.csv`
- `data/unyo_土日祝.csv`

### GitHubへのアップロード手順

1. リポジトリのルートディレクトリに以下をアップロード:
   - `mobile.html`
   - `mobile.js`

2. `data/` フォルダは既存のものをそのまま使用

3. ファイル構成:
```
tosaden-phone/
├── mobile.html          ← 新規追加
├── mobile.js            ← 新規追加
├── index.html           (既存)
├── monitor.js           (既存)
├── online_monitor_6columns.html (既存)
└── data/
    ├── stops.txt        (既存)
    ├── stop_times.txt   (既存)
    ├── unyo_平日.csv     (既存)
    └── unyo_土日祝.csv    (既存)
```

### アクセス方法

**スマホ版:**
```
https://soutripo.github.io/tosaden-phone/mobile.html
```

**PC版（既存）:**
```
https://soutripo.github.io/tosaden-phone/
```

### 特徴

- **12列表示**: 東西線10列 + 南北線2列
- **行間**: PC標準の1倍（100px）
- **駅名**: 17px（大きめ）
- **縦スクロール**: 全12列を見られる
- **スマホ最適化**: タップしやすいUI

### 設定値

- 各列の高さ: 100px
- SVG全体: 1500px
- マージン: 上下30px、左右20px
- 駅名フォント: 17px（太字）
- 列車番号: 15px（太字）

### トラブルシューティング

**404エラーが出る場合:**
1. GitHub Actionsの完了を待つ（1-3分）
2. ブラウザのキャッシュをクリア
3. シークレットモードで確認

**表示がおかしい場合:**
1. ハードリフレッシュ（Ctrl+Shift+R）
2. 数分待ってから再度アクセス
