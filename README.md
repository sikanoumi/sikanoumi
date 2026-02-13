# 🌱 Yomi（ヨミ） | Applied AI Engineer（LLM × Memory × Evaluation）

LLMを「人格＝policy」として扱い、**Router / Memory / Eval** まで含めた再現可能な実験基盤と、プロダクト実装を両方やります。  
研究っぽい話を **動くデモ＋ベンチ＋metrics＋証拠ログ** で示すのが得意です。

## 🔥 Featured (Portfolio)
### ✅ NeuroLikeLab — persona router × MemGPT memory × AgeMem gate
LLMの「人格＝policy」を Router（state×task）で切替え、MemGPTメモリ＋AgeMem gate を **ベンチ＆metricsで再現可能に評価**した実験基盤です。
- Repo: https://github.com/sikanoumi/NeuroLikeLab  
- Release: `v0.3-router1`（router100 + persona breakdown + UI demo）  
- Evidence: fixed bench + fixed metrics snapshot + UI demo

## 🧠 Other Projects
- **YggPersonaBot（ユグペルソナボット）**  
  感情・記憶・人格を持つキャラクターAIを統合。状態管理と対話体験を設計・実装。
- **Persona LINE Bot**  
  LINE上で動くキャラクターBot。ユーザーごとの状態/人格/記憶を管理。

## 🧰 Stack
Python / FastAPI / GitHub  
LLM: OpenAI API / (local LLM)  
RAG: FAISS / Vector Search  
Memory: Redis  
Eval: JSONL metrics / reproducible benches  
Image Gen (optional): SDXL / LoRA

## 📫 Contact
GitHub: https://github.com/sikanoumi
