# BreastCancerDiagnosis
### 介紹
此專案中我們針對細針抽吸方式 FNA（fine needle aspirate)獲得的乳腺癌檢測的患者數據集，建立一預測模型。資料集的來源是開源資料集-[乳腺癌數據集](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))，每個患者的FNA數據是由多個細胞樣本中產生 10 個不同特徵的統計數據以及診斷結果（惡性或良性）表示。基於多篇論文、醫學專家下，在[Eickhoff (2016)](https://dl.acm.org/doi/pdf/10.1145/2594776.2594788?casa_token=GMtjoBep2nkAAAAA:7n4D47l-D5yDvNTHgw8KBqQwQd03KuJnYy3hXhBTKqv940MklIJFSsM0wuF4JA1wnL0qv3K3YDp_7g)論文中整理了5個判斷為惡性腫瘤的要點，我們根據這5要點作為模型設計、訓練的基準。在多項實驗後，我們使用了隨機森林分類器」獲得了最好的表現，avg precision: 97%，avg recall: 96，avg f1-score: 97。


### 介紹
[Eickhoff (2016)](https://dl.acm.org/doi/pdf/10.1145/2594776.2594788?casa_token=GMtjoBep2nkAAAAA:7n4D47l-D5yDvNTHgw8KBqQwQd03KuJnYy3hXhBTKqv940MklIJFSsM0wuF4JA1wnL0qv3K3YDp_7g)論文中基於「考慮到特定類型的組織，細胞的大小往往是均勻的」所設計的五要點為：
1) 存在明顯較大的細胞是不受控制的生長的證據，這表明惡性腫瘤。
2) 良性細胞的形狀通常僅顯示有限的差異，而惡性細胞可以發展出與其周圍環境的一般模式不相符的任意結構。
3) 相同類型的常規細胞的細胞核顏色應相同。癌細胞通常具有明顯更大且較暗的細胞核，DNA 更密集。
4) 規則細胞顯示出相似的紋理。另一方面，惡性腫瘤可以範圍從光滑的表面到相鄰細胞的參差不齊或塊狀紋理。
5) 最後，對於健康組織，細胞排列趨於有序，細胞之間的距離規則。癌細胞幾乎可以任意散開或雜亂無章。
