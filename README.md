# 🚀 Everyone AR Beam - Super Accurate AI Edition

ブラウザとカメラだけで楽しめる、超高精度な物体認識AIを搭載したARビームWebアプリです。

最新のディープラーニングモデル（TensorFlow.js / COCO-SSD）をブラウザ内で直接動作させることで、画面内の物体をリアルタイムに自動検知し、その中心へ向かって重厚感のある3Dプラズマビームを超精密にロックオン＆追従させます。

**👉 [今すぐデモを体験する](https://core315185.github.io/everyone-AR-beam/)**
*(GitHub Pagesにホストされています)*

![スナップショット](https://raw.githubusercontent.com/core315185/everyone-AR-beam/main/snapshot.png)
*(※ここにアプリの動作スクショやGIFがあれば配置してください)*

## 🌟 主な特徴

*   **🤖 AI自動物体認識**: Googleが開発したCOCO-SSDモデルを搭載。人、スマホ、ボトル、カップなど、COCOデータセットに含まれる **80種類の物体** をカメラにかざすだけで瞬時に自動認識します。
*   **🎯 超高精度ロックオン & 追従**: 以前の色パターン追従方式を廃止し、AIが計算した物体のバウンディングボックスの中心へ、ビームを正確に吸い付かせます。
*   **✨ 暴れ・チラつきの完全解消**: 移動平均フィルター（ローパスフィルター）を実装。AIの認識座標を平滑化することで、誤検知によるガタつきやチラつきを抑え、ぬるぬると滑らかに移動するビームを実現しました。
*   **🔥 重厚な3Dビームエフェクト**: Three.jsを使用し、太く強力なコア（芯）とゆらぐプラズマオーラを持つ、存在感のあるビームを3D空間に描画します。
*   **🌐 完全ローカル・プライバシー対応**: すべてのAI処理はWebブラウザ内（TensorFlow.js）で完結します。カメラ映像はサーバーに送信されないため、安心して利用できます。

## 🛠 遊び方

1.  **URLにアクセス**: スマホ（iOS/Android推奨）またはPCのブラウザでデモページを開きます。
2.  **カメラの許可**: ブラウザからカメラへのアクセス許可を求められるので、「許可」してください。
3.  **AIロード（初回のみ）**: 最初に「AI物体認識モデルをロード中...」と表示されます。10秒〜20秒ほどかかりますので、そのままお待ちください（2回目以降はキャッシュされます）。
4.  **ロックオン開始**: カメラを人、スマートフォン、飲み物のボトルなどに向けます。
5.  **ビーム射出！**: AIが物体を検知すると、青い枠（デバッグ表示）が現れ、その中心へ向かって自動的に強力なビームが照射され、物体が動いても追従します。
6.  **カメラ切替**: 画面下の「📷 カメラ切替」ボタンで、インカメラとアウトカメラを切り替えられます。

## 📋 推奨動作環境

ディープラーニング処理をブラウザで行うため、比較的新しい端末が推奨されます。

*   **iOS**: iPhone 11以降、iOS 15以上、Safari推奨
*   **Android**: ハイエンドCPU搭載端末、Chrome推奨
*   **PC**: GPUを搭載したChrome / Edge / Safari

## 🔧 使用している主要技術

*   **AI (Object Detection)**: [TensorFlow.js](https://www.tensorflow.org/js) / [COCO-SSD model](https://github.com/tensorflow/tfjs-models/tree/master/coco-ssd)
*   **3D Rendering**: [Three.js](https://threejs.org/)
*   **Camera Handlers**: [MediaPipe Camera Utils](https://github.com/google/mediapipe)
*   **Language**: HTML5 / JavaScript (ES6+)

## 📄 ライセンス

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
COCO-SSD and TensorFlow.js are licensed under the Apache License 2.0.

## 👋 作者

*   [core315185](https://github.com/core315185)