---
layout: post
title: knight-of-heavenly-palace
categories: works
tags: works
permalink: /works/knight-of-heavenly-palace
image: /assets/src/knight-of-heavenly-palace/TitleLogo.png
image2: /assets/src/knight-of-heavenly-palace/TitleLogo.png
---

# 天上宮殿の騎士
---

## 概要

### 使用言語
C#

### 主要ツール
- Unity 2021.2.15f1
- Rider
- GitHub
- UniRx
- UniTask

### 主要開発人数

| 役職 | 人数 |
| ---- | ---- |
| プランナー<br>(リーダー含む) | 3人 |
| プログラマー | 6人 |
| デザイナー | 7人 |

### 制作期間
2022/4/22 ～ 2022/09/23

---

## 担当&実装箇所

- Joy-Conの入力用のラッパークラス & 値の加工
- Joy-Conを降った時の角度の計算
- アニメーションマネージャーの作成
- 敵の挙動
  - ドラゴンの移動と攻撃の挙動
  - ザコ敵の移動の挙動
- エフェクトマネージャーの作成とそれを設定するエディターの作成
- エフェクト
  - 剣の投擲
  - 転移
  - 着地時の砂埃

---

### 実機プレイ映像
<iframe width="560" height="315" src="https://www.youtube.com/embed/0xTNXxZfsR0?si=UQ1VZ1qsgnT-4NC9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

実行デバイス : Nintendo Switch

---

## こだわり

### Joy-Conの処理
Nintendo SDKからJoy-Conの値を回収し、ゲーム内で使用しやすいように加工しました。\
ゲーム内でJoy-ConをWiiのリモコンのように使用しカーソルとして使用する場面があるのですが、そのJoy-Conからスクリーン座標に変換する計算なども担当しました。

---

### 敵の挙動
State駆動で敵の動きの処理を実装しました。\
Stateの割り込み機能を追加してプレイヤーを見失ったときなどにStateの切り替えをできるようにしました。

---

### GitHubリポジトリ
[knight-of-heavenly-palace-public](https://github.com/letconst/knight-of-heavenly-palace-public)\
実行にはNintendo SDKが必要です。

---