# ローカルLLMワークショップ

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hayatoshibahara/local-llm-workshop/blob/main/main.ipynb)

## 概要

**Ollama** を使ってローカル LLM を Google Colab 上で動かし、日本語での推論性能やエージェント機能を体験する初心者向けワークショップです。

LLM・ローカル LLM の基礎知識の座学から、Ollama SDK を使ったハンズオン（基本推論・ツール呼び出し・エージェントワークフローなど）まで、90分でひととおりカバーします。

## アジェンダ

1. **LLM とは** — 概要・変遷、Transformer・Attention・トークン予測の仕組み
2. **ローカル LLM** — 導入背景、代表モデル、パラメータ数・量子化・GGUF・Dense vs MoE・Thinking モード、推論エンジン比較
3. **LLMハンズオン**
    - セットアップ（Ollama インストール・サーバー起動・モデルダウンロード）
    - 基本的な推論（日本語性能の確認）
    - システムプロンプト
    - マルチターン会話
    - ストリーミング
    - 構造化出力（JSON）
    - ツール呼び出し（Open-Meteo 天気 API 連携）
    - パラメータ調整（temperature・top_p・frequency_penalty）
    - エージェントワークフロー（ルーター → スペシャリスト → ガードレール）
4. **まとめ** — 学習内容の振り返り、発展トピック（ファインチューニング・RAG・LangGraph）