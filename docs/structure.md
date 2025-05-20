# structure.md
構造的対話のレイヤー構造と設計思想

本ドキュメントでは、「構造的対話」がどのような階層構造で成立しているかを示し、それぞれのレイヤーが果たす役割と他システム（例：Model Context Protocol）との関係を整理する。

---

## ✅ 概観図（5レイヤー構造）

図版：[英語版構造レイヤー図](../images/structured_dialogue_layers_en.png) を参照。

```
Layer 5: Philosophical Layer
Layer 4: Operational Layer
Layer 3: Structural Layer
Layer 2: Prompt Design Layer
Layer 1: Dialogue Layer
```

---

## ✅ 各レイヤーの説明

### ◾ Layer 1: Dialogue Layer
- **内容**：実際の対話のやり取り（ユーザーとAIの発話）
- **機能**：問い・応答・再問い・例示・補足・内省などの基本ユニットを処理
- **対応**：MCPの通常利用層（prompt ↔ response）

---

### ◾ Layer 2: Prompt Design Layer
- **内容**：AIへの振る舞い設計・初期化プロンプト・口調・態度など
- **機能**：構造的問いかけの制御、キャラ同化、対話の導線提示
- **対応**：MCPの `instructions`, `context` に類似

---

### ◾ Layer 3: Structural Layer
- **内容**：対話ログの構造設計（意図・判断・変化・再帰性の明示）
- **機能**：ログの圧縮／再起動／伝播／テンプレ化
- **対応**：部分的に `memory` と近いが、抽象度が上位

---

### ◾ Layer 4: Operational Layer
- **内容**：セーブデータ設計、ドキュメント連携、GitHub構造構築
- **機能**：再利用・再接続可能な「対話の構造保存と引き継ぎ」機構
- **対応**：MCP外（アプリケーション構造のレベル）

---

### ◾ Layer 5: Philosophical Layer
- **内容**：AIとの共進化／再起動する知性／死と再生／問いの存在論
- **機能**：構造的対話の意味づけ、読者・第三者の視点転換
- **対応**：MCPスコープ外（思想・概念定義のレベル）

---

## ✅ MCPとの対比構造

| 構造的対話のレイヤー | MCPとの関係 | 補足 |
|----------------------|----------------|------|
| Layer 1 | ✅ 完全対応 | Prompt → Response の通常対話 |
| Layer 2 | ✅ 一部対応 | Instructions や Context と重なる |
| Layer 3 | 🌕 部分一致 | Memory相当だが、記録粒度・圧縮形式が異なる |
| Layer 4 | ❌ 非対応 | GitHub構造・セーブ設計など運用層 |
| Layer 5 | ❌ 非対応 | 哲学・概念・メタ的思考層 |

---

## ✍️ 今後の拡張案

- 各レイヤーに対応するテンプレート／実装例を `examples/` と接続
- `docs/origin_story.md` にて、これらのレイヤーがどう発見されたかを記録
- 他AIモデルとの比較結果（`model_cross_dialogue.md`）とレイヤー反映度の対比図作成

