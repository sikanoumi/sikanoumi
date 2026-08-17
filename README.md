# SIKANOUMI | Applied AI / LLM Engineer

生成AIを「使える機能」に落とし込むために、  
**LLM Evaluation / RAG / Fine-tuning / Agent / Product Engineering** を軸に実験と実装を行っています。

LLMをAPIで呼び出すだけではなく、

**dataset design → baseline → retrieval / fine-tuning → evaluation → error analysis**

まで含めて、結果を比較・検証できる環境を作ることを重視しています。

また、AI機能単体だけでなく、**認証・UI・API・AI・デプロイ**まで含めたWebアプリケーション実装にも取り組んでいます。

---

# 🔥 Featured Projects

## ✅ Closed-World LLM Benchmark
### Base vs RAG vs QLoRA vs RAG + QLoRA

未公開のオリジナル架空世界を使い、  
**Base / RAG / QLoRA / Hybrid** を同一条件で比較したLLM評価プロジェクトです。

40問 × 4条件 = **160回答をblind human evaluation**し、  
Fact / Reasoning / Unknown / World Boundary に加えて、

- Unsupported Claim
- Hallucination
- Outside-world Leakage
- Latency

を独立して評価しました。

* Repo: https://github.com/sikanoumi/closed-world-llm-benchmark
* Model: `Qwen/Qwen3.5-9B`
* Embedding: `Qwen/Qwen3-Embedding-0.6B`
* Reranker: `Qwen/Qwen3-Reranker-0.6B`
* Highlights: RAG / QLoRA / PEFT / FAISS / Reranker / Blind Evaluation / Reproducible Benchmark

### Result

| Condition | Fact | Reasoning | Hallucination |
|---|---:|---:|---:|
| Base | 0.042 | 0.000 | 10.0% |
| RAG | 0.833 | 0.600 | 52.5% |
| QLoRA | 0.042 | 0.000 | 17.5% |
| Hybrid | **0.875** | **0.700** | 40.0% |

今回の条件では、QLoRA単体によるClosed-World QA性能の改善は確認できず、  
**RetrievalがFact / Reasoning性能に大きく寄与**しました。

一方でRAGによって回答可能性が高まるとUnsupported Claim / Hallucinationも増えることが分かり、  
**CorrectnessとGroundingを分離して評価する必要性**も確認しました。

---

## ✅ TalkSeed — AI-assisted 1on1 support app

1on1ミーティングを支援するためのWebアプリケーションです。

**Next.js / FastAPI / Microsoft Entra ID / Azure** を用いて、  
認証、相手選択、AI話題提案、メモ管理、PDF出力などを実装しました。

AI機能だけではなく、**認証・Frontend・Backend API・Cloud Deploymentまで含めたProduct Engineering**を行っています。

* UI Repo: https://github.com/sikanoumi/talkseed-ui
* API Repo: https://github.com/sikanoumi/talkseed-api
* Highlights: Next.js / TypeScript / FastAPI / Entra ID / Azure / AI Integration / PDF Export

---

## ✅ japanese-llm-tuning-lab
### Japanese LLM Evaluation & LoRA Tuning

日本語の会議メモ・業務メモから、決まったJSON形式で  
**要約 / 決定事項 / ToDo / リスク** を抽出するためのLLM評価・LoRAチューニング実験です。

`Qwen/Qwen2.5-0.5B-Instruct` を使用し、

**baseline evaluation → dataset design → LoRA fine-tuning → before/after comparison → error analysis**

まで実施しました。

* Repo: https://github.com/sikanoumi/japanese-llm-tuning-lab
* Highlights: Local LLM / LoRA / PEFT / Dataset Design / Structured Output Evaluation

### Result

| Metric | Before | After |
|---|---:|---:|
| schema_valid_rate | 0.1250 | **0.8750** |
| todo_owner_accuracy | 0.0000 | **0.6875** |
| todo_due_accuracy | 0.0000 | **0.8125** |
| hallucination_flag_rate | 0.8750 | **0.1250** |

---

# 🧪 Other Projects

## NeuroLikeLab — persona router × memory × eval

LLMの応答スタイルを **persona = policy** として扱い、  
Router（state × task）で切り替えながら、MemoryとEvaluationを組み合わせる実験基盤です。

* Repo: https://github.com/sikanoumi/NeuroLikeLab
* Release: `v0.3-router1`
* Highlights: Router / Memory / Evaluation / Metrics / UI Demo

---

## Inner Palette — non-judgmental color flow interface

自由記述をラベルやスコアではなく、  
**個人固有の色の流れ**として返す非裁定インターフェースです。

Next.js / FastAPI / SQLiteで、入力・分析・履歴表示まで含むMVPを実装しました。

* Repo: https://github.com/sikanoumi/inner-palette
* Highlights: AI × UI / Personalized Palette / History / Interaction Design

---

# 🧰 Stack

### LLM / Applied AI

- OpenAI API / Azure OpenAI
- Hugging Face Transformers
- Qwen
- LoRA / QLoRA / PEFT
- RAG / FAISS / Vector Search
- Embedding / Reranker
- Agent / Router / Memory
- LLM Evaluation / Error Analysis

### Backend

- Python
- FastAPI
- Pydantic
- SQLite
- Redis

### Frontend

- Next.js
- TypeScript
- React

### Auth / Cloud

- NextAuth
- Microsoft Entra ID
- Microsoft Graph
- Azure
- Azure App Service

### Development

- Git / GitHub
- VS Code
- Claude Code
- JSONL-based evaluation pipelines

---

# 🎯 Focus

- Applied AI / LLM Engineering
- RAG / Retrieval / Reranking
- LLM Evaluation & Grounding
- LoRA / QLoRA Fine-tuning
- Agent / Memory Design
- AI × Backend / Product Engineering
- Evaluation-first Development

---

# 📫 Contact

* GitHub: https://github.com/sikanoumi
