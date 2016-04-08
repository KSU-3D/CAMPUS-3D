Welcome to the CAMPUS-3D wiki!
# CAMPUS-3D まとめwiki

このwikiにはCAMPUS-3Dでのキャンパスデータ（3Dモデル）の作成方針を示していきます。

## 作成の際のテクニック
リアリティに見せるための工夫として，繰り返し使い回せるオブジェクト（椅子や机や置物など），または大きなオブジェクト（建物など）．細かい部分はとことん妥協する．
特に植物系は作るのが面倒なので，Unityのアセットストアから手に入れるようにする，そのほかにも使えそうなオブジェクトはなるべく使う．ただし、ダウンロードしたポリゴン数は念のため確認を
下の学習サイトのような玄人や公式サイトなどから""手法を盗む(マネる)""，たまに本屋で業界本を立ち読みもありかも．

## 学習サイト
Blender Guru(作者: Andrew Price) https://www.youtube.com/user/AndrewPPrice
Tornardo Twins(作者: Tornardo) https://www.youtube.com/user/TornadoTwins
brackeys.com (作者:brackeys) http://brackeys.com/
SpreadBlender(作者:日本人)https://www.youtube.com/user/SpreadBlender

## Unityに関するWebサイト
unity terrain how to make  https://www.youtube.com/watch?v=tlix0Sb7LLQ

## パフォーマンス（意外と影響する）
DrawCall（テクスチャの呼び出し回数）とポリゴン数を気にしないといけない．
DrawCallを少なくする方法は、なるべく同じマテリアルの使い回し、テクスチャをモジュールごとに一つの画像ファイルにまとめるようにする．
ポリゴン数は曲線をなるべく使わないようにし、できる限りテクスチャで細かな凹凸を表現する．
コンシューマゲームのキャラクターのポリゴン数は，主人公で1万〜2万，敵キャラで数千であり，iPhoneで実装するときはもう少し抑える必要があるので，ググってみて業界のポリゴン数を見た方が良い．
リアルタイムでの表示/非表示のローディングはUnityのカメラコンポーネントのClippingPlanesで調整できるが、さらにローディングでのメモリ管理を考える場合は質のレベルが違うオブジェクトを複数用意し、距離に応じて対応させる必要がある。→ Unityのオクルージョンカリングという機能でカバーできるかも
↑の参考サイト　GravityDaysにおけるオープンワールドの作り方http://sekigames.gg-blog.com/Entry/243/
	

##【Bumpマッピングテクスチャのためのソフトウェア】
CrazyBump

##【テクスチャ関連のサイト】
http://www.textures.com
テクスチャペイント向けの画像も含めあらゆる素材が揃っているサイト。(要ユーザ登録)
(サイズの大きな画像は有料ですが、無料サイズの画像でも十分な画質だと思います)

##【Unity Asset Store - 使えそうなアセット】
植物
「GreenLeaf - Tree Pack 2」
「Realistic Tree Pack」
「Big Nature Pack」
土、地面、地盤、石
テクスチャ
「Factures pack for Unity5」
