---
layout: post
title: "EnigMouse"
categories: works
tags: works
permalink: /works/EnigMouse/
image: /assets/src/EnigMouse/TitleLogo.png
---

# EnigMouse

### GitHubリポジトリ
ゲーム本編\
[EnugMouse](https://github.com/to3oi/EnigMouse_Public)

入力装置\
[EnigMouseSendMaster](https://github.com/to3oi/EnigMouseSendMaster)\
[EnigMouseSendClient](https://github.com/to3oi/EnigMouseSendClient)

### ストーリー
プレイヤーは魔法学校の生徒。
授業中誤って二次元に封じ込める魔法を暴走させ、教室の鍵を封印してしまう。
教室から出るために他の生徒と協力し、鍵を入手して教室から脱出しよう。

## 担当&実装箇所
ゲーム本編
- 入力周りの処理
- 入力装置との通信
- ゲームの進行
- マスを切り替える処理などを考慮したクラス設計
- 一部のエフェクト
- 残り時間のUI
- いくつかのマネージャークラスの作成\(InputManager,EffectManager,GameManager,TitleManager)

入力装置すべて
- ゲーム本編との通信
- Azure Kinect DKを使用した画像処理
- 物体検出

その他
- プロジェクターとAzure Kinect DKと机の距離の調整
