# プロジェクト構成概要（Structure Overview）

このドキュメントでは、本リポジトリのディレクトリ構成と、各ファイル・サブディレクトリの役割を説明します。

---

## 📁 ルートディレクトリ

```
/
├― README.md               # 英語版の概要ドキュメント（国際向け）
├― README_ja.md           # 日本語版の概要ドキュメント（実質的なメイン）
├― LICENSE                # ライセンス（MIT）
├― docs/                  # 補足ドキュメント群
├― examples/              # 応用例・再現例（ログやテンプレート）
├― images/                # 図片・視観資料
└― prompt_templates/      # プロンプトの再利用テンプレート群
```

---

## 📁 docs/

構造的対話に関連する解説・FAQ・応用法をまとめたドキュメント群。

* `structure.md`（このファイル）: ディレクトリ構成の解説
* `prompt_examples.md`: 実際に使用されたプロンプトのサンプル集
* `use_cases.md`: 構造的対話の応用事例（業務・創作・教育等）
* `faq.md`: よくある質問と回答

---

## 📁 examples/

実際に行われた構造的対話のログやテンプレートを保存。

* `structure_log.md`: 対話ログにおける文脈構造の記録
* `detroit_energy_log.md`: 「ブルーブラッド」のエネルギー構造に関する検証ログ
* `agent_prompt_test.md`: 他AIへの適用検証例など

---

## 📁 prompt\_templates/

プロンプトの汚用テンプレートを格納。再利用や応用が可能。

* `structured_thinking_base.txt`: 構造的思考を支援する基本プロンプト
* `dialogue_engineering_prompt.yaml`: 対話型AIに向けた制御ルールの例
* `creative_character_mode.md`: キャラクター設定の構造化テンプレ

---

## 📁 images/

構造的対話の概念図、構造図などを格納。

* `flowchart_structured_dialogue.png`: 構造的対話のプロセス図
* `diagram_usecase_matrix.png`: 応用領域のマトリクス図（予定）

---

## 🔚 備考

* ディレクトリ・ファイル名は英語統一（国際展開を見据えた設計）
* 日本語ドキュメント（README\_ja.md）は実質的な起点・母艦として設計
