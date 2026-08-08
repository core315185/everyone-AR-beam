Everyone AR Beam (誰でもARビーム)
カメラにかざした「手（指先）」からインタラクティブな3D ARビーム（パーティクルエフェクト）を発射するWebARアプリケーションです。

特殊なアプリのインストールは不要で、PCやスマートフォンのブラウザからURLを開くだけで動作します。

🌟 Webアプリ（公開URL）
以下のURLからすぐにブラウザで遊ぶことができます。

👉 https://core315185.github.io/everyone-AR-beam/

🌟 特徴
リアルタイム手認識: MediaPipe Handsを使用し、指先の位置を高速かつ高精度にトラッキング
3Dパーティクル描画: Three.jsを活用したリアルタイムなビームエフェクト表現
動的Web Audio効果音: 外部音声ファイルを使わず、JavaScriptで効果音をリアルタイム生成
マルチデバイス対応: PC（Webカメラ）およびスマートフォン（iOS / Android）のインカメラ・アウトカメラに対応
🚀 使い方
公開済みの GitHub Pages URL にアクセスします。
ブラウザから「カメラへのアクセス」を求められたら 「許可」 を選択します。
カメラに手をかざすと、指先からARビームが描画され、効果音が流れます。
🛠️ 技術スタック
HTML5 / CSS3 / JavaScript (ES6+)
Three.js: 3Dレンダリングおよびパーティクルシステムの構築
MediaPipe Hands: 機械学習による手・指のキーポイント検出
Web Audio API: 音声ファイルの読み込みなしで効果音を直接生成
💻 ローカル環境でのテスト方法
リポジトリをクローンまたはZipでダウンロードします。
git clone [https://github.com/core315185/everyone-AR-beam.git](https://github.com/core315185/everyone-AR-beam.git)
