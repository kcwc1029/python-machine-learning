Part 1：資料前處理 Data Preprocessing
│
├── Features 與 Target
├── 缺失值處理
├── 類別資料編碼
│ ├── Label Encoding
│ └── One-Hot Encoding
├── Train / Test Split
├── Feature Scaling
│ ├── Standardization
│ └── Normalization
└── sklearn 基本工作流程

快速介紹一下機器學習流程

- [快速介紹一下機器學習流程](./快速介紹一下機器學習流程/快速介紹一下機器學習流程.ipynb)

資料前處理

- [Data Preprocessing](./data_preprocessing/data_preprocessing.ipynb)

迴歸 Regression

- [Simple Linear、Multiple Linear and Polynomial](./regression/regression.ipynb)
- [Support Vector Regression](./SVR/SVR.ipynb)
- [Decision Tree Regression](./Decision_Tree_Regression/Decision_Tree_Regression.ipynb)
- [Random Forest Regression](./Random_Forest/Random_Forest.ipynb)

分類 Classification

- [Logistic Regression](./Logistic_Regression/Logistic_Regression.ipynb)
- [Classification Evaluation Metrics](./Classification_Evaluation_Metrics/Classification_Evaluation_Metrics.ipynb)
- [KNN](./KNN/KNN.ipynb)

分群 Clustering

- [K-Means](./K-Means/K-Means.ipynb)

關聯規則 Association Rule Learning

- [Apriori](./Apriori/Apriori.ipynb)

降維 Dimensionality Reduction

- [PCA](./PCA/PCA.ipynb)

模型選擇 Model Selection

- [Model Selection](/Model_Selection/Model_Selection.ipynb)

Ensemble & Boosting

- [Ensemble Learning & Boosting](./Ensemble_Learning_&_Boosting/Ensemble_Learning_&_Boosting.ipynb)

幫我寫一份【】的教材，內容要教

Part 8：Ensemble & Boosting
│
├── Ensemble Learning 基本概念
├── Bagging
├── Random Forest 再深入
├── AdaBoost
├── Gradient Boosting
└── XGBoost

- 白話理解原理，不用遷入到過多數學
- 以快速上手運用為主，要所以解釋要參數
- 跑模型的資料及，也要準備給我

沒有章節/時長限制，以品質/完整度為第一優先，我當然會希望一份教材越充實完整越好
程式碼要註解
可以適時放一些示意圖進去(沒有要你生成，你就幫我寫好提示詞就好，後續我在自己另外慢慢生成圖片即可)
圖片大小16:9 尺寸1280 × 720，要給我圖片名稱

程式碼部分，大致可以分為

- 讀取資料集
- 選擇 Features 與 Target
- 切分 Train / Test
- 建立模型
- 訓練模型
- 使用模型預測
- 評估模型表現
- 視覺化預測結果
- 出一份作業，請參考下列：

```text
## 作業：使用 Random Forest Regression 預測臺灣空氣品質指標 (AQI)

本次作業使用政府資料開放平臺提供的「空氣品質指標(AQI)(歷史資料)」，並使用 Random Forest Regression (隨機森林迴歸) 建立模型，預測臺灣各空氣品質監測站的 AQI 數值。

\- 資料集：[空氣品質指標(AQI)(歷史資料)]\([https://data.gov.tw/dataset/151824](https://data.gov.tw/dataset/151824))

模型根據空氣中的污染物濃度與氣象條件，例如：

\`\`\`text
PM2.5 細懸浮微粒濃度
PM10 懸浮微粒濃度
O3 臭氧濃度
NO2 二氧化氮濃度
SO2 二氧化硫濃度
CO 一氧化碳濃度
風速
\`\`\`

預測：
\`\`\`text
AQI 空氣品質指標
\`\`\`

建立以下關係：
$$
\boxed{
\text{空氣污染物與氣象數據}
\longrightarrow
\text{Random Forest Regression}
\longrightarrow
\text{預測 AQI}
}
$$

AQI 本身就是依污染物監測數值計算出來的指標，因此這次作業主要訓練學生使用 Random Forest 重建數值關係，並不是預測未來的空氣品質。

學生必須按照以下順序完成：
\`\`\`text
1. Pandas 讀取政府開放資料
        ↓
2. 查看資料 (head / info / describe)
        ↓
3. 資料清理
        ↓
4. 選擇 Features / Target
        ↓
5. Train / Validation / Test Split
        ↓
6. 建立資料前處理 Pipeline
   (SimpleImputer / StandardScaler / OneHotEncoder)
        ↓
7. 建立模型
        ↓
9. 訓練模型
        ↓
10. 使用模型進行預測
        ↓
11. 評估模型表現
        ↓
12. 視覺化
\`\`\`

請參考格式與水準，幫我為羅基回歸也出一份
資料及也是要政府資料開放平臺提供的(資料及要不同的)
```
