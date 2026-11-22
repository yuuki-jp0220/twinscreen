# TwinScreen

スマートフォン・パソコン向けのブラウザ画面共有ページです。

## 公開方法
1. GitHubリポジトリの **Settings → Pages** を開く
2. **Deploy from a branch** を選択
3. Branch を **main**、Folder を **/(root)** にして Save
4. 数分後に `https://yuuki-jp0220.github.io/twinscreen/` で公開されます

## 接続方法
- 2台で同じページを開き、同じルームコードを入力します。
- 片方をA、もう片方をBにして接続します。
- 共有側で「画面共有を開始」を押し、ブラウザの共有許可を選びます。

## 対応・制限
- WebRTCとPeerJSの公開シグナリングサーバーを利用します。映像は原則として端末間で直接送信されます。
- ネットワークやNATの条件によっては接続できない場合があります。安定性を高めるにはTURNサーバーの設定が必要です。
- getDisplayMediaの対応状況はブラウザ・OS依存です。特にAndroidでは画面共有APIが利用できない端末・ブラウザがあります。
- GitHub PagesはHTTPSで配信します。画面共有APIには安全なコンテキストが必要です。
