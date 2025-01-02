使用六種方法進行訓練分析:
1. adaboost
2. xgboost / linear regression
3. lstm /cnn
4. Random Forest

使用下面兩種方法進行比較:  
1. 將全部資料使用pca降維
2. 透過model中的Regressor選前15個最重要的參數

資料前處理固定
各個model的參數自己嘗試最好的
1.	刪掉id、alley、MiscFeature、PoolQC和Fence
2.	數值na填平均
3.	類別na選眾數
4.	數值都要標準化(z-score)
5.	結果求MAE
