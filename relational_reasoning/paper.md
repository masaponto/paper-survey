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

## Introduction 

要素とその属性の間の関係を推論することは知能的な振る舞いの中心です。(Figure 1) [18, 15].

子供が公園の遠く離れた木々の間を走るときのことを考えて見ましょう、どこを走るかを知るために、公園の木々の間の距離を推論し、見比べなければなりません。
または、推理小説において、犯人推理するために、証拠を集める読者を考えてみましょう。もっともらしいストーリーとミステリーを解決するために、それぞれの手がかりはより広い文脈で考えられなければ.なりません。
AIを使った主なアプローチはInherently relational (関係推論)です。。

Symbolic approaches to artificial intelligence are inherently relational [32, 11]. 
Practitioners define the relations between symbols using the language of logic and mathematics, 
and then reason about these relations using a multitude of powerful methods, including deduction, arithmetic, and algebra.

But symbolic approaches suffer from the symbol grounding problem and are not robust to small
task and input variations [11]. Other approaches, such as those based on statistical learning, build
representations from raw data and often generalize across diverse and noisy conditions [25]. However,
a number of these approaches, such as deep learning, often struggle in data-poor problems where the
underlying structure is characterized by sparse but complex relations [7, 23]. Our results corroborate
these claims, and further demonstrate that seemingly simple relational inferences are remarkably


## Relational Question
