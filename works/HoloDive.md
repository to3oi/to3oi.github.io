---
layout: post
title: "HoloDive"
categories: works
tags: works
permalink: /works/HoloDive/
image: /assets/src/HoloDive/TitleLogo.png
image2: /assets/src/HoloDive/TitleLogo.png
---

# HoloDive

---

## 概要

### 使用言語
C#

### 主要ツール
- Unity	2021.3.3f1
- Rider	2022.2.4
- UniRx	6.2.2
- UniTask	2.3.2
- DOTween (HOTween v2)	1.2.705
- Mixed Reality Toolkit   2.8.2
- Vuforia	10.13.3

### 主要開発人数
プランナー : 3人\
プログラマー : 2人\
計5人

### 制作期間
2022/10/05 ~ 2023/2/11

---

## 実装箇所
Hololens 2本体で使用するコード
- 環境構築
- ゲームの進行管理
- 画像認識した画像の種類の通知処理
- エフェクトなどの演出

[コードの確認はこちら](https://github.com/to3oi/HoloDive-Hololens-Repository-Public/tree/main/Assets/User/Tomoi)

---

---

## 実機動画
<iframe width="560" height="315" src="https://www.youtube.com/embed/smT1GH2vxLM?si=OTHXEV5NACUT993s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

実行デバイス : Hololens 2

---

---

## ストーリー
過去と未来に干渉する研究をしているあゆむ研究所。\
プレイヤーはこの研究所の研究員。\
時空干渉デバイスHoloDiveをかぶりあゆむ研究所の爆発を止めよう！

---

---

## 操作方法
- プレイヤーは左手の手の甲を右手の人差し指で2回タップすることで時間を移動できます。
- 現在の時間が過去か未来かを確認するには左手の手の甲のマークの色で確認できます。
青で過去、赤で未来の時間にいます。
- チュートリアルのモニターを確認して内容をの通りに操作、移動してください。

---

---

## こだわり

### 時間軸の移動
手の甲を2回タップすることで時間軸を移動する事ができます。\
この処理をするためにMRTKで取得できる指と手の甲の位置に動的にコライダーを配置し、タップの検出ができるようにしました。

![](../assets/src/HoloDive/HoloDive_FingerTrigger.png)

---

### 時間軸移動時のエフェクト
以下の動画のように時間軸を移動したときに、手の座標を中心に波紋のようなエフェクトを実装し、時間軸を移動したことをプレイヤーがわかるようにしました。\
初期のものはビルドして実行するとFPSが5程度しか出ず実用的ではありませんでした。
しかし調べてみるとFragment Shaderの値が大きいことが原因ということがわかりこの値を減らせるよう負荷の重いSample Noiseをより軽量なGradient Noiseへ置き換え、Hololens 2上では影響の少ないAlphaの処理をなくすことで最大30FPSを出せるよう修正できました。


<iframe width="560" height="315" src="https://www.youtube.com/embed/smT1GH2vxLM?si=HGrpoBMENT7A1oYb&amp;start=32" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


---

---

### GitHubリポジトリ
[HoloDive-Hololens-Repository-Public](https://github.com/to3oi/HoloDive-Hololens-Repository-Public)

[![HoloDive](https://github-readme-stats.vercel.app/api/pin/?username=to3oi&repo=HoloDive-Hololens-Repository-Public)](https://github.com/to3oi/HoloDive-Hololens-Repository-Public)

---