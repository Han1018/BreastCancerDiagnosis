# BreastCancerDiagnosis
### 介紹
此專案中我們針對細針抽吸方式 FNA（fine needle aspirate)獲得的乳腺癌檢測的患者數據集，建立一預測模型。資料集的來源是開源資料集-[乳腺癌數據集](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))，每個患者的FNA數據是由多個細胞樣本中產生 10 個不同特徵的統計數據以及診斷結果（惡性或良性）表示。基於多篇論文、醫學專家下，在[Eickhoff (2016)](https://dl.acm.org/doi/pdf/10.1145/2594776.2594788?casa_token=GMtjoBep2nkAAAAA:7n4D47l-D5yDvNTHgw8KBqQwQd03KuJnYy3hXhBTKqv940MklIJFSsM0wuF4JA1wnL0qv3K3YDp_7g)論文中整理了5個判斷為惡性腫瘤的要點，我們根據這5要點作為模型設計、訓練的基準。在多項實驗後，我們使用了隨機森林分類器」獲得了最好的表現，avg precision: 97%，avg recall: 96，avg f1-score: 97。





### Dataset
The file wdbc.pkl  Download wdbc.pklcontains a dataset of patients tested for breast cancer using a fine needle aspirate (FNA). Each patient is represented by statistics of 10 different features of multiple cell samples, as well as a diagnosis (malignant or benign). For definitions of these variables, see [Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)) Dataset. The file wdbc.pkl  Download wdbc.pklhas columns in the order: subject id, label, features. Clarification: The three different features for each variable, with suffixes "_0", "_1", "_2" represent the mean, standard deviation and "worst" value over a set of samples, respectively. Please see the ["Data description"](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names) for a precise definition.
