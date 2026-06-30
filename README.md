# SIKANOUMI | Applied AI / LLM Engineer

生成AIを「使える機能」に落とし込むために、**LLM Evaluation / LoRA Tuning / Agent / RAG / Memory** を軸にした実験と実装に取り組んでいます。

個人開発では、LLMをただAPIで呼び出すだけではなく、
**dataset design / baseline evaluation / fine-tuning / before-after comparison / error analysis** まで含めた再現可能な検証環境を作っています。

プロダクト寄りでは、**認証・UI・API・AI機能・デプロイ** まで含めて、
実運用を見据えたWebアプリケーションの設計と実装を行っています。

---

## 🔥 Featured Projects

### ✅ japanese-llm-tuning-lab — Japanese LLM evaluation & LoRA tuning

日本語の会議メモ・業務メモから、決まったJSON形式で **要約 / 決定事項 / ToDo / リスク** を抽出するための、LLM評価・LoRAチューニング実験リポジトリです。

`Qwen/Qwen2.5-0.5B-Instruct` を使い、baseline推論、LoRA fine-tuning、before / after比較、error analysisを行いました。

* Repo: https://github.com/sikanoumi/japanese-llm-tuning-lab
* Highlights: local LLM / LoRA / dataset design / JSON schema evaluation / error analysis
* Result:

  * `schema_valid_rate`: `0.1250 → 0.8750`
  * `todo_owner_accuracy`: `0.0000 → 0.6875`
  * `todo_due_accuracy`: `0.0000 → 0.8125`
  * `hallucination_flag_rate`: `0.8750 → 0.1250`

### ✅ NeuroLikeLab — persona router × memory × eval

LLMの応答スタイルを **persona = policy** として扱い、Router（state × task）で切り替えながら、
MemGPT型メモリと AgeMem gate を組み合わせて **再現可能な評価** を行う実験基盤です。

* Repo: https://github.com/sikanoumi/NeuroLikeLab
* Release: `v0.3-router1`
* Highlights: router / memory / evaluation / UI demo / metrics snapshot

### ✅ TalkSeed — AI-assisted 1on1 support app

1on1 ミーティングを支援するための Web アプリケーションです。
Next.js / FastAPI / Entra ID を用いて、相手選択、AI話題提案、メモ管理、PDF出力まで含む体験を実装しました。

* UI Repo: https://github.com/sikanoumi/talkseed-ui
* API Repo: https://github.com/sikanoumi/talkseed-api
* Highlights: Next.js / FastAPI / Entra ID / Azure App Service / AI topic suggestions / PDF export

### ✅ Inner Palette — non-judgmental color flow interface

自由記述をラベルやスコアではなく、**個人固有の色の流れ**として返す非裁定インターフェースです。
Next.js / FastAPI / SQLite で、入力・分析・履歴表示まで含む MVP を実装しました。

* Repo: https://github.com/sikanoumi/inner-palette
* Highlights: AI × UI / personalized palette / history / quiet interface

---

## 🧰 Stack

* **Backend**: Python / FastAPI
* **Frontend**: Next.js / TypeScript / UI prototyping
* **Auth**: NextAuth / Microsoft Entra ID
* **LLM**: OpenAI API / local LLM / Hugging Face Transformers
* **Fine-tuning**: LoRA / QLoRA / PEFT
* **RAG**: FAISS / Vector Search
* **Memory**: Redis / structured memory design
* **Evaluation**: JSONL metrics / schema validation / reproducible benches / error analysis
* **Infra / Tools**: Azure / Azure App Service / GitHub / SQLite / VS Code

---

## 🎯 Focus

* Applied AI / LLM feature implementation
* LLM evaluation and structured output improvement
* LoRA / QLoRA fine-tuning experiments
* Agent / RAG / Memory design
* Evaluation-first development
* Turning AI systems into usable product experiences

---

## 📫 Contact

* GitHub: https://github.com/sikanoumi
