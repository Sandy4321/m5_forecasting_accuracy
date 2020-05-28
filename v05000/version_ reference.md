# Version Reference

- 特徴量エンジニアリングや目的関数の調査が滞ってきたので、モデリングの方式を変える。


## Experiments
- v05000
  - v04000 の複製
- v05001
  - リファクタリング
- v05002
  - storeごとにモデルを学習し、予測を行う。
- v05003
  - deptごとにモデルを学習し、予測を行う。
- v05004
  - v05002 を踏襲
  - いくつか特徴量を追加する
    - lag 特徴量追加 7, 14,-> 1~14
    - target encoding
- v05005
  - v05003 を踏襲
  - いくつか特徴量を追加する
    - lag 特徴量追加 7, 14,-> 1~14
    - target encoding

### TODO
- v05006
  - `train_data[train_data['release'] < 30]` を除去
- v05007
  - 特徴量選択
- v05008
  - Hierarchical Bayesian Target Encoding の実装