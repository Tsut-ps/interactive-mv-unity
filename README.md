# もう、とけた。

![image](https://github.com/user-attachments/assets/ae3b6502-6a32-4c28-ba15-67cd7895b2df)


[「もう、溶けた。」 - Mealerrand より](https://www.youtube.com/watch?v=GRR_35gxZho)  

いつの日かのプロトタイプ「もう、とけた。」  
バージョン: 0.40  


## 概要
演奏できる (体験できる) ワールド  
楽器を鳴らす (有効化する) と後ろの音が増える  


## 特徴
- 一人称視点 (いずれVRでもやってみたいわね)
- 音楽が流れる
- ゲームを進める
  → 音楽が進む  
  → 楽器が増える  


## MVの「動画」以外の可能性を探りたい

音楽は聴く。  
動画は見る。  
Webページは動かせる。  

ならば、動くWebページで音楽を体験できたらどうだろう。  

![image](https://github.com/user-attachments/assets/07a88584-41e9-48a2-8b5a-512e779c148a)

音楽、自分から体験できたら もっと面白くできるのでは……？  

![image](https://github.com/user-attachments/assets/a5de3eb2-fa15-4d5c-9127-357a9d40d17f)


## 基本操作

- マウス: 視点操作
- WASDキー: 移動
- Eキー/左クリック: ドアの操作 / 楽器の操作

![image](https://github.com/user-attachments/assets/7234b279-1471-412c-9f66-035c6de10c19)


## 苦労したところ / 工夫したところ

- 90%はC#とUnityの仕様に困惑した (URPとBP)
- 操作感上の問題からVSCodeで開発した  
  → 環境構築に難ありだけど、めちゃくちゃ軽い
- 音声周りのロジック  
  → タイミングに悩まされる (音が毎回ズレる……など)
- 再生中は特定の行動ができないように (別の音源を流すなど)
- どの端末でも画面内に収めるレスポンシブ対応 (PWA化すると画面いっぱいになる)
- ちょっとした遊び心 (なぜ楽器は踊る)
- WebGL周りのブラウザキャッシュにご注意 (ビルド時に反映されないことがある)
- 構想を除けば、全体を通して一週間で開発した

![image](https://github.com/user-attachments/assets/b6e052d0-f050-4ebe-889d-f775ba6d7ad9)


## まだまだ改善できそうなところ

- WebGLにのみ見られる光漏れ
- 音源が一括管理じゃない (アイテム化して所持してもよさそう)
- 音源が再生される条件が複雑でスパゲティコード
- 「暁」のところでアニメーションしてやはり窓から日がさしていてほしい （もっと歌詞と照らし合わせたい）
- 低スペックだと発生する音源の音ズレをなんとかしたい  
  CRIWAREをよく見るが……
- スクリプト内に重複して書いている部分が多すぎる
- 楽器の音量調整が不可逆


## 素敵な楽曲

Mealerrandさんの「もう、溶けた。」のStemデータを使用しています 
- 動画: [YouTube](https://www.youtube.com/watch?v=GRR_35gxZho)
- Stemデータ: [Googleドライブ](https://drive.google.com/drive/folders/14QbLbf7RW3Z2zGTVb-rcptAd8ss-zQlq)
- 利用規約: [note](https://note.com/mealerrand/n/nfd1f698e81bc)

## 補足
- GitHubにアップロードする際、100MBを超えるファイルはリポジトリに含められないため、ある程度テクスチャを圧縮しました (サイズ: 2048 → 1024 など)
- このWebアプリの正式名称は「もう、とけた。」が正しいです。途中、いろいろな解釈ができると判明し、私も制作にあたってとけまくったのです
