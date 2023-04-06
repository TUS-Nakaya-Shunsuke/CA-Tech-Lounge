# CA-Tech-Lounge

CA Tech Loungeの提出型課題における進捗を以下に記録する.  
期限は2023/04/19 23:59までだが, 私用によりどうしても 2023/04/13 ~ 2023/04/18 は課題を行うことができない.  
限られた時間で可能な限りのことをする.


## 2023/04/05
- gitのセットアップ
- README.md, .gitignoreの追加
- Covertype Data Set, Data Description の確認
    - データ数 : 581012
    - 特徴量 : 54
        - 量的変数 : 10, バイナリ質的変数(自然保護区分類) : 4, バイナリ質的変数(土壌タイプ分類) 40
    - ラベル : 7
    - Train : 11,340, Valid : 3780, Test : 565892 における分類精度
        - Neural network : 70%
        - Linear Network : 58%
- covtype.csvの作成
- 課題の問題設定に関する質問

## 2023/04/06
- covtype_input.csv, covtype_target.csvの作成
- 問1
    - Train : 11,340, Valid : 3780, Test : 565892 で分析&評価
    - Random Forest を用いて実行
    - Cross Validationの手法の検討
        - KFold (Shuffle=True or False)
        - StratifiedKFold (Shuffle=True or False) : 採用
- 予測精度のベースラインを決定
