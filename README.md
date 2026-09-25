# ゼロから作るDeep Learning ❻ 学習リポジトリ

書籍『[ゼロから作るDeep Learning ❻ —LLM編](https://www.amazon.co.jp/dp/4814401612)』（オライリー・ジャパン）を読みながら、LLMの仕組みを理解するために自分でコードを書いている個人の学習用リポジトリです。

本書の公式リポジトリではありません。公式のソースコードは次のリポジトリで公開されています。

- https://github.com/oreilly-japan/deep-learning-from-scratch-6

## ファイル構成

| パス | 内容 |
| :-- | :-- |
| `ch01/`〜`ch07/`, `ch09/` | 各章で自分が書いたコード（8章はコードなし） |
| `AGENTS.md` | AIエージェントに学習を手伝ってもらうときの指針 |

答え合わせ用に公式リポジトリを手元の `reference/` にコピーしていますが、このリポジトリには含めていません（`.gitignore` で除外）。

## 環境

- Python 3.12（[uv](https://docs.astral.sh/uv/) で管理）
- 依存ライブラリは公式リポジトリの `requirements.txt` に合わせています（PyTorch 2.x、NumPy 1.x、Matplotlib、tqdm、regex、wandb）
- オプションで openai、tiktoken

```bash
# 環境構築
uv sync --extra full

# 実行
uv run python ch01/xxx.py
```

答え合わせに公式コードを使う場合は、公式リポジトリを `reference/` に置いてください。
