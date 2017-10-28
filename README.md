# TakeU
### tk_1714

[![TakeU](https://raw.github.com/GabLeRoux/WebMole/master/ressources/WebMole_Youtube_Video.png)](https://www.youtube.com/channel/UC4PtjOfZTbVp9DwtJv82Lzg)

## 製品概要
### 地図を見ながらの歩きスマホ　X Tech

### 背景（製品開発のきっかけ、課題等）
#### プロダクトの開発に至った背景
- 旅行が趣味→新しい土地を歩くことが多い→スマホでマップを確認することが多い
    -  安全性：治安が悪い場所でスマホに集中するのは危ないと感じた
    - よりよい旅行体験：もっと街を見ながら歩きたい

#### 着目した顧客
- 地図を見ながら歩きスマホする人々

#### 顧客の課題
- 言わずもがな歩きスマホは危険
- 音声入力も聴覚が遮られてしまい危険

#### 現状
- 首都圏の鉄道利用者のうち歩きスマホする人の割合は50.5%<sup>[1]</sup>
    - そのうち地図アプリの利用者は42.3%<sup>[1]</sup>
- 移動する際に地図アプリを使う人の割合は54.9%に上る<sup>[2]</sup>
    - 特に我々の世代(18-29歳)は69.1%も<sup>[2]</sup>
- 10/25にホノルルで歩きスマホ禁止条例が施行された<sup>[3]</sup>
- 旅行先だけでなく、日常生活でも地図を見る機会は多い
    - 知らない居酒屋に行くとき
    - 集合場所に行くとき
    - 東大前から2号館に行くとき
- Googlemap等の音声ガイダンスもあるが聴覚が遮られてしまい危険

### 製品説明（具体的な製品の説明）
-「地図と現実をシームレスにつなぐ」をコンセプトにした、"振動"によって目的地までガイドするネックレス型デバイス。
- スマホのアプリで目的地を設定しナビゲーションをスタートさせる。

### 特長

#### 1. 特長1 ユニバーサルデザイン

#### 2. 特長2 低コスト

#### 3. 特長3 ...?

### 解決出来ること
- 歩きスマホからの解放
- より一層周りを見ながら歩くことができる
- 方向音痴でも直感的に歩くことができる

### 今後の展望
- 三叉路の対応
- ネックレス型のプロダクトをスタイリッシュにする
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
    * Speech Framework
    
#### デバイス
* iPhone

### 研究内容・事前開発プロダクト（任意）
ご自身やチームの研究内容や、事前に持ち込みをしたプロダクトがある場合は、こちらに実績なども含め記載をして下さい。

*
*


### 独自開発技術（Hack Dayで開発したもの）
#### 2日間に開発した独自の機能・技術
* 独自で開発したものの内容をこちらに記載してください
* 特に力を入れた部分をファイルリンク、またはcommit_idを記載してください（任意）


---

## 参考文献
[1]一般社団法人電気通信事業者協会(2017)「『やめましょう、歩きスマホ。』に関する調査」(URL:http://www.tca.or.jp/press_release/pdf/170308sumahochosa.pdf)<参照2017-10-28>
[2]株式会社ゼンリン(2017)「地図利用実態調査」(URL:http://www.zenrin.co.jp/dl/pdf/material06.pdf)<参照2017-10-28>
[3]NHK(2017)「ハワイ ホノルルで「歩きスマホ」禁止条例施行 | NHKニュース」(URL:http://www3.nhk.or.jp/news/html/20171026/k10011198601000.html)<参照2017-10-28>
