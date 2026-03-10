# 🌱 Yomi（ヨミ） | Applied AI Engineer

生成AIを「使える価値」に変えるために、**Agent / RAG / Memory / Evaluation** を軸とした実験基盤とプロダクト実装に取り組んでいます。  
個人開発では、**Router / Memory / Eval** を含む再現可能な検証環境を作り、**動くデモ + bench + metrics + evidence log** で改善を進めています。

## 🔥 Featured Project
### ✅ NeuroLikeLab — persona router × memory × eval
LLMの応答スタイルを **persona = policy** として扱い、Router（state × task）で切り替えながら、  
MemGPT型メモリと AgeMem gate を組み合わせて **再現可能な評価** を行う実験基盤です。

- Repo: https://github.com/sikanoumi/NeuroLikeLab
- Release: `v0.3-router1`（router100 + persona breakdown + UI demo）
- Evidence: fixed bench + fixed metrics snapshot + UI demo

## 🧠 Other Projects
- **YggPersonaBot**  
  感情・記憶・人格を持つキャラクターAIを統合し、状態管理と対話体験を設計・実装。
- **Persona LINE Bot**  
  LINE上で動作するキャラクターBot。ユーザーごとの状態・人格・記憶を管理。

## 🧰 Stack
- **Backend**: Python / FastAPI
- **Frontend**: UI demo / Web app prototyping
- **LLM**: OpenAI API / local LLM
- **RAG**: FAISS / Vector Search
- **Memory**: Redis
- **Evaluation**: JSONL metrics / reproducible benches
- **Optional**: SDXL / LoRA

## 📫 Contact
- GitHub: https://github.com/sikanoumi
