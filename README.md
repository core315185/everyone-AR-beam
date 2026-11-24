⚡ Everyone AR Beam (Next-Gen HTML5 Edition)

Webカメラで撮影した手や指先を Google MediaPipe Hands でリアルタイムにAI認識し、指先をタップしてロックオンすると、指先から3D空間へ向かって力強いプラズマ発光の光の柱（ARビーム）が滑らかに延長・追従する最先端WebARアプリケーションです。

特殊なアプリのインストールは一切不要で、スマートフォンのブラウザ（Safari / Chrome）やPCのブラウザで直接動作します。

🚀 アプリの起動方法

1. Web（GitHub Pages）から起動する（推奨）

リポジトリの設定で GitHub Pages を有効化すると、アプリ用URLが発行されます。

👉 ⚡ ARビームアプリを起動する

(※ <ユーザー名> と <リポジトリ名> はご自身のGitHubアカウント・リポジトリ名に置き換えてください)

2. ローカル環境で起動する場合

PCの場合: Visual Studio Codeの拡張機能 Live Server などを使用し、ローカルWebサーバー経由で index.html を開いてください。

スマホの場合: スマホのブラウザ（Safari / Chrome）からローカルサーバーURLにアクセスしてください。

🌟 主な機能と特徴

MediaPipe Hands による超高精度ハンドトラッキング:

手の21個の関節・指先（ランドマーク）をリアルタイムで認識。

タップ位置から最も近い指先（人差し指・親指などの先端）を自動判定してロックオンします。

フル画面追従 & アスペクト比補正:

カメラ映像の object-fit: cover による切り取り領域を自動計算し、指の動き・位置・角度の変化にビームの根元と方向がピタリと滑らかに追従します。

次世代プラズマ発光ビーム & 加算合成:

Three.js (WebGL) を駆使し、中心が眩しく輝く高輝度コアと外側発光コア、さらに舞い散るスパークパーティクルをリアルタイム描画。

完全シングルファイル（Single-File Component）設計:

HTML、CSS、JavaScript、外部AIライブラリの連携をすべて index.html の1ファイルに凝縮し、高い移植性と軽量性を実現。

🎮 使い方

アプリを起動し、「🚀 システム起動」 ボタンをタップ。

カメラへのアクセス許可ダイアログが表示されたら 「許可」 を選択。

カメラに手をかざし、画面上の指先をタップするとARビームが発射・追従します！

操作ボタン

❌ 1本解除: 最後に発射したビームを1本削除します。

🗑 全削除: 画面上のすべてのビームを消去します。

🛠 技術スタック

フロントエンド: HTML5, CSS3, JavaScript (ES6+)

3D描画エンジン: Three.js (WebGL / 加算合成マテリアル)

AIハンドトラッキング: Google MediaPipe Hands

カメラアクセス: MediaDevices API (navigator.mediaDevices.getUserMedia)

📦 ファイル構成

.
├── index.html     # WebGL 3D AR & プラズマ発光追従アプリ本体（単一ファイル構成）
└── README.md      # 本ドキュメント


⚠️ 動作環境・注意事項

推奨ブラウザ:

iOS: Safari

Android / PC: Google Chrome

カメラ機能およびMediaPipeライブラリの通信には HTTPS環境（または localhost）が必要です。