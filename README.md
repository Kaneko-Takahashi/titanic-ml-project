```markdown
# 🚢 Titanic ML Project - タイタニック生存予測

機械学習（scikit-learn）を使用したタイタニック号の乗客生存予測プロジェクト

## 📋 プロジェクト概要

Kaggleの有名なデータセット「Titanic」を使用して、二値分類（生存/死亡）の機械学習モデルを構築します。

## 🛠️ 環境構築手順

### 1. リポジトリのクローン

```bash
git clone https://github.com/Kaneko-Takahashi/titanic-ml-project.git
cd titanic-ml-project
```

### 2. 仮想環境の作成と有効化

```bash
# 仮想環境作成
python -m venv venv

# 有効化（Windows）
venv\Scripts\activate

# 有効化（Mac/Linux）
source venv/bin/activate
```

### 3. 必要なライブラリのインストール

```bash
pip install -r requirements.txt
```

### 4. 動作確認

```bash
# notebooks/01_setup_test.ipynb を実行して環境を確認
```

## 📁 フォルダ構成

```
titanic-ml-project/
├── data/ # データファイル格納
├── notebooks/ # Jupyter Notebook
│ ├── 01_setup_test.ipynb # 環境確認用
│ ├── 02_data_exploration.ipynb # データ探索・可視化
│ └── 03_preprocessing.ipynb # 前処理・モデル構築・評価
├── src/ # Pythonスクリプト
├── outputs/ # 出力結果（グラフなど）
│ ├── age_distribution.png # 年齢分布グラフ
│ ├── survival_by_gender_class.png # 性別・クラス別生存率
│ └── confusion_matrix.png # 混同行列グラフ
├── .gitignore # Git管理除外設定
├── requirements.txt # 必要ライブラリ一覧
└── README.md # このファイル
```

## 🔧 使用技術

| 技術 | バージョン | 用途 |
|------|-----------|------|
| Python | 3.11.5 | プログラミング言語 |
| pandas | 2.2.3 | データ操作・分析 |
| numpy | 1.26.4 | 数値計算 |
| scikit-learn | 1.5.2 | 機械学習 |
| matplotlib | 3.9.2 | グラフ描画 |
| seaborn | 0.13.2 | 統計グラフ描画 |
| jupyter | 1.1.1 | インタラクティブ開発環境 |

## 📊 プロジェクトの進行状況

- [x] STEP 1: 環境構築
- [x] STEP 2: データ取得と確認（探索的データ分析）
- [x] STEP 3: 前処理（特徴量エンジニアリング）
- [x] STEP 4: モデル構築（ロジスティック回帰・ランダムフォレスト）
- [x] STEP 5: 評価（混同行列・各種スコア）
- [ ] STEP 6: 改善（ハイパーパラメータチューニング）

## 📈 分析で判明した傾向

- 全体の生存率は約38.4%
- 女性の生存率が男性より大幅に高い
- 上流クラス（1st）ほど生存率が高い
- 子供の生存率が高い（Women and children first）
- 年齢（age）に欠損値あり → 前処理で対応が必要

## 🎯 学習目標

1. **分類問題**の基本的な流れを理解
2. **scikit-learn**の実践的な使い方を習得
3. **前処理**の重要性と手法を学習
4. **モデル評価**の各種指標を理解
5. **GitHub**でのプロジェクト管理を実践

## 📝 License

MIT License

## 🔗 参考リンク

- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- [scikit-learn Documentation](https://scikit-learn.org/)
- [pandas Documentation](https://pandas.pydata.org/)
```
