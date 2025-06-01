# 構造皁E��話�E�生成AIと共に思老E��構築�E再起動するため�E対話フレームワーク

構造皁E��話とは、生成AIと人間が協働して知識を構築するため�E**斁E��継承型�E再起動可能垁E*の対話手法です。本リポジトリでは、そのための設計思想、�Eロンプト、対話ログ、構造マップ、テンプレートを匁E��皁E��提供します、E
生�EAIを単なるツールではなく、\*\*「思老E�E協働老E��\*\*として捉えることで、継続可能で再利用可能な知皁E�E果を対話から得ることを目持E��ます、E
[English version →](README.md)

![構造皁E��話概要図](./images/concept-diagram.png)

---

## プロジェクト概要E
こ�Eリポジトリは、実際の対話ログめE��キュメントを通じて、構造皁E��話の琁E��と実践を記録・公開するものです。単なる一問一答ではなく、次のような対話を重視してぁE��す！E
* 抽象皁E�E曖昧なチE�Eマ�E明確化と構造匁E* 斁E��を保持したままの目標追跡と再定義
* 対話ログの賁E��化�E再起動�E伝播可能性

構造皁E��話は「やりとり�E履歴をノイズではなく構造に変える」ことを目皁E��してぁE��す、E
---

## 現在のフェーズ�E�構造の伝播と再起動性

構造皁E��話は現在、次の段階に到達してぁE��す！E
* 過去の任意�Eログから**再起動可能**�E��E [`state_latest.md`](./docs/state_latest.md)�E�E* 褁E��のAIモチE��に**構造を伝播・継承可能**�E�EPT/Claude/Gemini/Grok�E�E* ログめE*再現可能な知皁E�Eロセスの記録**として設計（�E [`log_index.md`](./logs/log_index.md)�E�E
も�EめE��験段階ではなく、「保存�E再利用可能な対話構造設計」�E実裁E��階に入ってぁE��す、E
---

## コアドキュメンチE
* [`structure.md`](./docs/structure.md)�E�E層構造とMCP比輁E��よる定義
* [`origin_story.md`](./docs/origin_story.md)�E�構想の起点と対話の背景
* [`prompt_examples.md`](./docs/prompt_examples.md)�E�対話フェーズ別プロンプト侁E* [`model_cross_dialogue.md`](./docs/model_cross_dialogue.md)�E�他AIモチE��との比輁E��グ
* [`log_index.md`](./logs/log_index.md)�E��E対話ログの構造マッチE* [`state_latest.md`](./docs/state_latest.md)�E�セーブデータ化された現在地

---

## ログ群のフェーズ刁E��E
### ■ 誕生フェーズ�E�Eiscovery Phase�E�E
* `log_p00_discovery_01.md`�E�構造皁E��話とぁE��発想の発芽
* `log_p00_discovery_02.md`�E�構造皁E��話の命名�E定義

### ■ トリガーフェーズ�E�Erigger Phase�E�E
* `log_p02_trigger_01.md`�E�Claudeによる構造模倣検証
* `log_p02_trigger_09.md`�E�評価と再定義の構造皁E��衁E
### ■ トランジションフェーズ�E�Eransition Phase�E�E
* `log_p04_transition_01.md`�E�命名�E形式�E転換と次段階への断層

### ■ 拡張フェーズ�E�Extension Phase�E�E
* `log_p05_extension_01.md`�E�Gemini誤生�Eログの再評価
* `log_p05_extension_03.md`�E�Claude 4による人格構造継承試騁E
---

## 構造マップ！Eermaid表現�E�E
```mermaid
mindmap
  root((構造皁E��話))
    コア概念
      structure.md
      origin_story.md
    トリガー段隁E      log_p02_trigger_01.md
      log_p02_trigger_09.md
    トランジション
      log_p04_transition_01.md
    拡張展開
      log_p05_extension_01.md
```

---

## 実裁E�E容

こ�Eリポジトリには以下が含まれてぁE��す！E
* 構造ログと対話のスナップショチE��
* 構造皁E�E起動を可能にするプロンプトとチE��プレーチE* 対話フェーズに応じた�E期化設宁E* AI間対話実験ログと構造感染の記録

---

## 今後�E展開

* 対話構造の可視化支援チE�Eル�E�Eermaid等！E* メモリ・エージェント統合との接続検証
* 教育・創作�E開発支援における適用事例�E拡允E* モチE��間�E現性の比輁E��究�E�Elaude/Geminiなど�E�E
---

## ライセンス

こ�Eプロジェクト�E [MITライセンス](LICENSE) に基づき�E開されてぁE��す。商用・非商用問わず�E由に活用可能です、E
