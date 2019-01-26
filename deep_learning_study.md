# Relational netwrokの紹介

# A simple network module for relational reasoning
- NIPS 2017
- deep mind
- https://arxiv.org/abs/1706.01427

## Abst
- 関係推論は知能的な振る舞いの中心の分野であるが、既存のニューラルネットワークでは学習が困難であることが知られる。
- Relational Network(RN)という関係推論を行うモジュールを提案
- RNをいれたネットワークで3つのタスクを検証した。
  - Visual QA tsak (CLEVR) で 構成度(当時SOTA)を達成
  - Text QA task (bAbI) super human なスコアを達成
  - 動的な物理シミュレーションシステムで複雑な関係推論を試した。　　
- Sort-of-CLEVRデータセットを用いてCNNにRNを加える事で高い精度がでることを示した
- 我々の研究は Relatinal Networkのモジュールを既存のdeep neural networkに追加することで、要素の関係を学習できることを示した。

## Relational Question


# Memory networks
- 過去の中間表現をメモリとして保存しておき、それを利用して推論する


# Working Memory Networks: Augmenting Memory Networks with a Relational Reasoning Module 
- https://arxiv.org/abs/1805.09354

## 概要
- 近年Deep Learning を用いた複雑な関係推論を解く手法が提案されている。
- 関係推論を行うため、Memory Networkは外部メモリとAttention機構を組み合わせた手法である。
- しかしながら、これらのアーキテクチャはより複雑な関係推論は困難である。
- 一方でRelation Networks (RNs)は関係推論のタスクにおいて飛び抜けた結果を出した。
- 残念なことに、このRNは複雑な問題においては、メモリの使用量など大きな計算コストが2次的にに上がってしまう。(オブジェクト同士の全組み合わせを計算するため)
- この問題を解決するために、我々はWorking Memory Network (MemNN アーキテクチャ)を提案する。そしてそれはワーキングメモリとRNモジュールを組み合わせたものである。
- 本手法はRNsを導入しているが、計算コストの増加を二次的でなく線形的に削減する。
- 我々は本モデルをbAbIデータセットとvisual QAデータセットのNLVRで検証した。
- 結果、MSEが0.5%以下でSOTAを達成。
- さらに、我々のシンプルなモデル2つのアンサンブルすることで、joint版のベンチマーク20タスクすべてを解く事に成功した。

## Intro
- 日常生活のタスクを解決するために必要な中心的な機能は複雑な関係推論である。
- それは、環境を理解、表現し、過去の経験から学習し、蓄えられた情報から問題を解決するということである。
- 私達人間のそれらの問題を解く能力は、複数の特別な機能からできています。
  - 短期記憶、長期的意味記憶、手続き記憶、そしてそれらの記憶を操作するAttention機構。
- 近年、複雑な関係推論を行うニューラルネットワークが多数提案されています。
- Deep Learningは複雑な(関係)推論のためのシンボル的アプローチではなく、知覚情報からの表現を学習することができます。
- そのため、Deep Learningはシンボルグラウンディング問題に直面することなく、シンボルを分類していくアプローチより、良い一般化が可能です。
  - シンボルグラウンディング問題とは記号システム内のシンボルがどのようにして実世界の意味と結びつけられるかという問題
- これらのNeural Network の多くのモデルは、メモリ(記憶装置)や、Attention機構を使います。
- Memory network, dyanamic memory network, Neural Tuning Machine (NTM) は 入力からのメモリと学習されたAttention機構によるメモリアクセスからなる。
- いくつかのメモリの記憶にAttention機構によって注意が向けられた後、複数ステップの手続きにより、注意が向いた記憶は(入力データと)結合され、最終結果を出力する出力層に流れます。
- これらのいくつかのプロセスの間に、networkは複雑な推論情報メカニズムが欠如してしまう。
   - そしてそれは、エンティティ(オブジェクト)の関係を推論(Relational Reasoning)するようなタスクにおいて必要な情報である。
- 一方で、Santoroによって提案されたRelational Network(RNs)は関係推論において高い性能が確認されました。
- Relational Networkの欠点はそれぞれ入力オブジェクトのペア(二乗的な組み合わせ関係)を考えなくてはならないこと。
- この欠点は、複雑なタスクに対してへの適用可能性に制限をかけてしまうし、また、順伝播、逆伝播に高い計算コストがかかる。
- この問題を解決するために、memory networkアーキテクチャのひとつである、Working Memory Networks (W-MemNN)を提案する。
- 我々はオリジナルのMemory NetworkにRNモジュールと新しいワーキングメモリバッファを追加した。

- Attention機構は



## WHAT’S THE CORE IDEA OF THIS PAPER?

## WHAT’S THE KEY ACHIEVEMENT?

## Experiment


## Future works

## Possible Business Applications

## WHAT ARE POSSIBLE BUSINESS APPLICATIONS?
