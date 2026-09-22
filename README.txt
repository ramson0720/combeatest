SORT! 1・2・3！ CPU横固定 UI改善版

変更点
- CPU対戦専用（2人対戦/スコアアタックをゲームモードから除外）
- 1点/2点/3点ボタンを横一列に配置
- CPU側の仕分けボタンを完全削除
- CPU表示を「残り枚数＋小さな山札」だけに縮小
- お題条件のアイコンを大きく表示
- ゲーム画面をスクロールしない固定レイアウトに変更
- manifest.webmanifest に orientation: landscape を指定
- 対応ブラウザでは Screen Orientation API で landscape lock を試行

iPhoneについて
Safariの通常タブではWebページ側からOSの画面向きを強制変更できない場合があります。
ホーム画面に追加したPWAで manifest の landscape 指定が効く環境では横向き起動を要求できます。
確実なOSレベルの横向き固定が必要ならネイティブアプリ化が必要です。

GitHubへは index.html / manifest.webmanifest / sw.js の3ファイルを更新してください。
