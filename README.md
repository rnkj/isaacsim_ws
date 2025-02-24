# Workspace for IsaacSim

## 概要
Motor babblingの事前学習のために、GPU並列化可能なシミュレーション環境構築を目指す。

Universal Robots UR5e, UFactory xArm7, ALOHAをはじめ、単腕・双腕の操作やシミュレーション環境の定義・表示を学習することを目的とする。

本ワークスペースで学習した内容はmotor babblingの学習実験にフィードバックし、まずは単腕での探索的な事前学習・テレオペレーションデータによる模倣学習の継続学習に適用する。

## チェックリスト
本ワークスペースでは下記の達成を目指す：
* URDF, MJCFの操作
    - [x] UR5e + Robotiq 2F-85のURDF表示
    - [x] Google-researchのPlayroomsをMJCF表示
    - [ ] URDF + MJCFの表示
    - [ ] ローカルディレクトリからmaterial (texture)をロードする
    - [ ] UR5eをインタラクティブマーカで操作
    - [ ] UR5eおよびグリッパへ指令値を送り操作
    - [ ] UR5eによる環境物の操作テスト
* 強化学習の設計
    - [ ] IsaacSim (IsaacLab)での強化学習スキームの学習
    - [ ] PyTorchによるPolicyを設計し、UR5eを操作（学習なし）
    - [ ] （強化学習のサンプルを試す）
    - [ ] 自作の強化学習モデルの準備とIsaacへの導入
    - [ ] Isaac上での訓練、訓練したpolicyのによる動作テスト
    - [ ] 並列環境の導入
    - [ ] 並列環境での学習・動作テスト
* 模倣学習の設計
    - [ ] IsaacLabでの模倣学習スキームの学習
    - [ ] 学習データの収集スキーム
        - [ ] 3Dマウス
        - [ ] （GELLO）
    - [ ] 学習データの収集
    - [ ] 模倣学習の実施
    - [ ] 訓練したpolicyのロードと動作テスト

各項の詳細は[PROGRESS.md](PROGRESS.md)にてまとめる。

## 環境
* Ubuntu 22.04 LTS
* Python 3.10
* IsaacSim 4.5.0

## Author
Ryoichi Nakajo

Last update: Feb. 24th, 2025.
