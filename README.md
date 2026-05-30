# ローカルLLMワークショップ

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hayatoshibahara/local-llm-workshop/blob/main/main.ipynb)

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
    - Google ColabでOllamaをインストールしてサーバーを起動
    - Qwen3.5:4Bモデルをダウンロード
    - Ollama SDKを使用した基本的な推論と日本語性能の確認
    - システムプロンプトによるモデルの挙動制御
    - マルチターン会話による文脈の保持
    - ストリーミングによるリアルタイムな応答表示
    - 構造化出力（JSON形式）による確実なデータ取得
    - ツール呼び出し（Tool Use）: Open-Meteo天気APIとの連携
    - temperature, top_p, frequency_penaltyなどのパラメータ調整
    - シンプルなエージェントワークフロー（ルーターAgent → スペシャリストAgent → ガードレールAgent）
1. まとめ
    - 学習した内容をまとめて解説
    - Unslothによるファインチューニング, RAG, Lang Graphによる状態管理などの発展を紹介
    - LLMの仕組みをより知りたい人向けにKarpathyのnanochatを紹介