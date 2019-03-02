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
