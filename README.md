---
marp: true
paginate: true
---
# ChatGPTでフロー開発を簡単に
2023年7月20日 横井一仁

https://kazuhitoyokoi.github.io/node-red-chatgpt

---
## 横井 一仁 (よこい かずひと)
- Node-RED開発メンバ
  - GitHubコミット数 世界3位
  - 和訳や不具合修正で貢献
- Node-RED User Group運営メンバ
  - Node-RED Con運営
  - UG Enterprise運営
- 日立製作所
  - ソリューションアーキテクト
  - DX、Industry 4.0研修講師
![w:400 bg right](https://nodered.jp/images/yokoi.jpg)

---
# 月刊I/Oの半年間の連載を完走しました🏃‍♀️💨📚
 - 3月号: プロジェクト機能の概要
 - 4月号: プロジェクトの切り替え
 - 5月号: フローのバージョン管理
 - 6月号: GitHubへフローを共有
 - 7月号: GitHubからフローを取得
 - 8月号: フローをクラウド環境へ<br>　 　　デプロイ
![bg right](https://pbs.twimg.com/media/FplCZZnaUAcopKn?format=jpg&name=large)

---
# 本日の内容
ChatGPT APIを活用したノードとプラグインを紹介
 - フローの作成手順のチュートリアル生成プラグイン
 - フローのドキュメントを生成するプラグイン
 - 文章からJavaScriptコードを生成できるfunctionノード

---
# ChatGPTでできること
Node-REDで活用できるChatGPTの機能
- 「作りたい物の説明文」から「フローのJSONデータ」を生成
- 「作りたい物の説明文」から「フローの作成手順」を生成
- 「フローのJSONデータ」から「フローの説明文」を生成
- 「フローのJSONデータ」からMermaid図を生成
- 「作りたい物の説明文」から「JavaScriptのコード」を生成

---
# フロー作成手順のチュートリアル生成プラグイン
開発したい物を入力するとエディタ上で開発手順を教えてくれるプラグイン

- ダイアログに作りたい物を入力しChatGPTで作成手順を生成
- ツアー機能を用いて、作成手順をステップバイステップで説明

https://twitter.com/kazuhitoyokoi/status/1647509785942827008

![bg right vertical](tutorial1.png)
![bg right vertical](tutorial2.png)

---
# フローのドキュメントを生成するプラグイン
開発したフローを説明する文章と図を<br>自動的に作成できるプラグイン

- フローの説明欄の下に「Ask ChatGPT」ボタンが追加される
- クリックすると、ChatGPTで生成した説明文を貼り付けてくれる

https://github.com/node-red-jp/node-red-contrib-plugin-chatgpt

![w:570 bg right vertical](https://raw.githubusercontent.com/node-red-jp/node-red-contrib-plugin-chatgpt/main/askchatgpt.png)
![w:570 bg right vertical](https://raw.githubusercontent.com/node-red-jp/node-red-contrib-plugin-chatgpt/main/infotab.png)

---
# 文章からJavaScriptコードを生成できるfunctionノード
functionノードの仕様に沿ったJavaScriptコードを生成するノード

- 作成したい物を入力後、<br>「Ask ChatGPT」ボタンを押す
- ChatGPTが生成したJavaScript<br>コードを貼り付けてくれる

https://twitter.com/kazuhitoyokoi/status/1653720620839104512

![w:630 bg right vertical](function.png)

---
## 感想
ChatGPT活用によって初心者ユーザ、ITエンジニア、OTエンジニアの距離が近くなった

 - Node-REDの初心者ユーザが、自身でハンズオンできるように
 - ITエンジニアは、分かりやすいドキュメントを提供できるように
 - ノーコード開発をしていたOTエンジニアが、ローコードの領域に踏み込めるように

![h:340](https://1.bp.blogspot.com/-Pnp3hqStlqw/XqUWuV_g7mI/AAAAAAABYjw/v5heWkhc4RMMNRH42JdTX37ToDNKsd07ACNcBGAsYHQ/s1600/online_school_boy.png) ![h:290](https://2.bp.blogspot.com/-Lm75_V4O7JY/V3x2OZbmIFI/AAAAAAAA8II/fzLckySfqnk0k7P-_YkSF8aDEBuUBodpQCLcB/s800/job_programmer.png) ![h:290](https://2.bp.blogspot.com/-756zNBRyNL8/VCkbkKOTRoI/AAAAAAAAnJA/zIJDGZopfCM/s800/koujou_kikai_sousa.png)
