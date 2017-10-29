# TakeU
### tk_1714

[![https://gyazo.com/b5cf1973ebdd09e7fc1d69baae456d12](https://i.gyazo.com/b5cf1973ebdd09e7fc1d69baae456d12.png)](https://gyazo.com/b5cf1973ebdd09e7fc1d69baae456d12)(https://www.youtube.com/watch?v=M-oKQlGpmaY)
## 製品概要
### 道案内 X Tech

### 背景（製品開発のきっかけ、課題等）
#### プロダクトの開発に至った背景
- 旅行が趣味→新しい土地を歩くことが多い→スマホでマップを確認することが多い
    - 安全性：治安が悪い場所でスマホに集中するのは危ないと感じた
    - よりよい旅行体験：もっと街を見ながら歩きたい
- そもそも地図を見ながら歩くことにストレスを感じていた
    - 前方不注意になり、人や自転車、車とぶつかる
    - 手に荷物を持っている時は使えない

#### 着目した顧客
- 地図アプリを見ながら歩くことに危険やストレスを感じている人たち

#### 顧客の課題
- 歩きスマホによる前方不注意
- 周りを見られないことによるストレス
- スマホ（地図）を持つことで手がふさがってしまう

#### 現状
- 首都圏の鉄道利用者のうち歩きスマホする人の割合は50.5%<sup>[1]</sup>
    - そのうち地図アプリの利用者は42.3%<sup>[1]</sup>
- 移動する際に地図アプリを使う人の割合は54.9%に上る<sup>[2]</sup>
    - 特に我々の世代(18-29歳)は69.1%も<sup>[2]</sup>
- 10/25にホノルルで歩きスマホ禁止条例が施行された<sup>[3]</sup>
- 旅行先だけでなく、日常生活でも地図を見る機会は多い
- Googlemap等の音声ガイダンスもあるが、それでは聴覚が遮られてしまうので危険

### 製品説明（具体的な製品の説明）
-「地図と現実をシームレスにつなぐ」をコンセプトにした、"振動"によって目的地までガイドするウェアラブルデバイス。
- スマホのアプリで目的地を設定しナビゲーションをスタートさせる。
- 左折、または右折するときには、その10m手前でデバイスが振動する。
    - 左折の時には左側の、右折の時には右側の振動モータが振動する。
- iPhoneとBluetooth通信をする
    - 独自に開発したアプリとの連携

### 特長

#### 1. 特長1 ：視覚や聴覚を遮ることなく、目的地までの道のりをガイドする

#### 2. 特長2 ：首にかけるデバイスなので、手を塞がない

#### 3. 特長3 ：操作方法がシンプル

### 解決出来ること
- 前方や周りを見ながら歩くことができる
- 手を塞がないで済む
- 景色を楽しむことができる
- 方向音痴でも直感的に歩くことができる

### 今後の展望
- ４叉路以上の場合の対応
- デバイスを小型化し、洗練されたデザインに
- Androidアプリの開発
- 地図のモード切り替え(徒歩・自転車)

## 開発内容・開発技術
### 活用した技術
#### API・データ

- Google Places API
- 固有表現抽出API (NTTレゾナント株式会社様より提供)

#### フレームワーク・ライブラリ・モジュール
* iOS: Swift
    * MapKit
    * CoreLocation
    * CoreBlutooth

#### デバイス
* iPhone
* BLE無線モジュール

### 研究内容・事前開発プロダクト（任意）

* デバイス
    * 無線モジュールの検討、テスト
    * デバイス設計

* アプリケーション
    * 実装方法の検討
        * GoogleMapAPI
        * CoreBlutoothのテスト

### 独自開発技術（Hack Dayで開発したもの）
#### 2日間に開発した独自の機能・技術

* 電信工作
  * モデリング(CAD)
  * はんだこて(飯室)
  * マイクロ

* デバイス
    * 外装のモデリング（Autodesk Fusion 360）、3Dプリント
    * デバイスの組み立て
    * マイクロコントローラ(C言語)

* アプリケーション
    * Bluetooth
      * アプリ起動時にバイブレーション
      * 右折、左折前にバイブレーション
      * ルート検索開始にバイブレーション
    * MapKitによる実装
        * マップ機能, 現在地情報の取得,ジオコーディング
        * 目的地の設定
          * 地名検索,補助機能(GooglePlacesAPI)
          * タップのジェスチャー
        * ルート検索機能
            * MapKit(MKDirections)による検索中のサジェスト
            * 2点間の距離に応じて縮尺を画面におさまるように
        * ナビゲーション機能
            * 現在地から目的地までの道順の配列をもとに方向と距離を取得
            * 曲がり角にジオフェンシング次の方向を取得し伝達

* 特に力を入れた部分をファイルリンク、またはcommit_idを記載してください（任意）


---

## 参考文献
[1]一般社団法人電気通信事業者協会(2017)「『やめましょう、歩きスマホ。』に関する調査」(URL:http://www.tca.or.jp/press_release/pdf/170308sumahochosa.pdf)<参照2017-10-28>
[2]株式会社ゼンリン(2017)「地図利用実態調査」(URL:http://www.zenrin.co.jp/dl/pdf/material06.pdf)<参照2017-10-28>
[3]NHK(2017)「ハワイ ホノルルで「歩きスマホ」禁止条例施行 | NHKニュース」(URL:http://www3.nhk.or.jp/news/html/20171026/k10011198601000.html)<参照2017-10-28>
