# ローカルLLMワークショップ

## 概要

エッジデバイス向けのLLMの性能を検証する初心者向けのワークショップ

## 前提

- Google Colabの無料プランで、VRAMが16GBのT5を使用
- 8B程度のSLMを使用し、日本語のエージェント性能を検証
- ワークショップの時間は90分
- 基礎知識の座学から雑務を処理するエージェントとしての活用までをカバーする

## 初期プラン

1. LLM
    - 概要: OpenAIなどのLLMの変遷
    - 仕組み: TransformerのAttention機構で次トークンの確率分布を計算してサンプリング
1. ローカルLLM
    - 導入: Macbook ProやJetson Nano Orinなどのエッジデバイスでの活用が高まっている背景
    - 種類: gpt-oss-120B, Qwen3-4Bなどの代表的なモデルの紹介
    - 基礎知識: Denseモデル、パラメータ数、量子化による性能低下と必要なメモリ要件
    - 推論エンジン: llama.cpp, Ollama, VLLM, LM Studioなどの紹介と選び方
1. LLMハンズオン
    - Google Colabで推論エンジンのインストールとモデルのダウンロード
    - OpenAI APIを使用してPythonスクリプトで推論し、日本語性能を確認
    - temperature, top_pなどのパラメータを解説
    - tool useなどのエージェントとしての機能を解説
1. まとめ
    - 学習した内容をまとめて解説
    - Unslothによるファインチューニング, RAG, Lang Graphによる状態管理などの発展を紹介
    - LLMの仕組みをより知りたい人向けにKarpathyのnanochatを紹介