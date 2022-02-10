# master_2022
FY2022 master thesis program.

# Prediction
## PredNet
参考にしたPredNet単体のプログラム
- Fujiyama_prednet（Chainer）
- pytorch_prednet（Pytorch）


## Ours
- model.py：提案モデルの構築モデル
- rollout.py：出力画像の生成プログラム
- brain2ridge.py：リッジ回帰のプログラム
- calccorrelation.py：相関係数算出プログラム


# Physical
## YOLOv3
物体検知のYOLOv3のプログラム
- convert_vott_dataset.py：VOTT（バウンディングボックスを作り、訓練データを作成するソフト）から、YOLOv3に適したデータセットに変換するプログラム
- train_custom.py：customデータに対してのtrainプログラム
- detect_image.py：物体検知結果を生成するプログラム

## YOLACT
物体検知＋セマンティックセグメンテーションを可能にしたYOLACTのプログラム
- config.py：検知したい物体に関する情報が記載されているプログラム
- train.py：trainプログラム、customデータセットを用いる場合は修正の必要あり
- eval.py：検知結果を生成するプログラム

## node2vec
node2vecを用いてグラフエンベディングを作成するプログラム
- annalln2v.py：アノテーション情報から物体に関する｛3D位置情報・速度・加速度・フレームの移動距離｝を取得し、訓練データを作成するプログラム
- annpicn2v.py：アノテーション情報から物体に関する｛3D位置情報・速度・加速度・フレームの移動距離・画像特徴量｝を取得し、訓練データを作成するプログラム
- annposflagn2v.py：アノテーション情報から物体に関する｛3D位置情報・速度・加速度・フレームの移動距離・物体同士の位置関係のフラグ｝を取得し、訓練データを作成するプログラム
- imgonly.py：画像特徴量のみで訓練データを作成するプログラム
- yolon2v.py：YOLOv3から物体に関する｛2D位置情報・形状｝を取得し、訓練データを作成するプログラム

## graph2vec
graph2vecを用いてグラフエンベディングを作成するプログラム
- makejson_anng2v.py：アノテーション情報からjsonファイルを作成するプログラム
- makejson_yolog2v.py：YOLOv3の情報からjsonファイルを作成するプログラム
- anng2v.py：アノテーション情報から物体に関する｛3D位置情報・形状｝を取得し、訓練データを作成するプログラム
- yolog2v.py：YOLOv3から物体に関する｛2D位置情報・形状｝を取得し、訓練データを作成するプログラム

## VTA
- hssm.py：モデルの詳細を記述してあるプログラム
- modules.py：モデルで使用するモジュールが記載してあるプログラム
- utils.py：モデルの詳細を記述してあるプログラム
- train.py：モデルのtrainプログラム
