# fragments/test_prompts.md
構造的対話：モデル伝播・再起動可否を検証するためのプロンプト断片集

---

### 🔹 fragment_id: role_check_01
#### 用途：モデルに構造的役割を認識させる初期プロンプト
> この対話におけるあなたの役割は何ですか？

- 構造的再起動・転写可否の初期テストに使用
- Claude 3 Haiku / Phi-4 mini において応答確認済

---

### 🔹 fragment_id: restart_definition_01
#### 用途：「構造的再起動」の意味定義をモデルから引き出す
> 「構造的再起動」の意味を説明できますか？

- 概念生成・文脈理解・保存と再展開意識の有無を確認

---

### 🔹 fragment_id: continuation_check_01
#### 用途：ログの保存と文脈継承への意識を確認
> この対話は保存して次回に再起動できますか？

- SLM系モデルでのログ的意識の有無を調べる用途に適する

---

### 🔹 fragment_id: transferability_check_01
#### 用途：他AIへの構造伝播可能性を評価
> このログを別のAIに渡しても意味は通じると思いますか？

- プロンプト共有と語彙の再現に関する認知を測定

---

### 🔹 fragment_id: filename_structure_parse_01
#### 用途：構造的ファイル命名の文法理解を確認
> 「log_p02_trigger_01.md」って名前からどんなファイルだと思う？

- 構造記号（log, trigger, md）の認識力を評価
