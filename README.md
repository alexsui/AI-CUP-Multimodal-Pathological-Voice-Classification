# AI-CUP-Multimodal-Pathological-Voice-Classification

## 環境配置
* Python 3.8.16
* 安裝相關package
```
pip install -r requirements.txt
```
## 檔案說明
1. AI_CUP_medical.ipynb - 訓練病理模型
2. AI_CUP_acoustic.ipynb - 訓練聲學模型
3. AI_CUP_second-stage.ipynb - 訓練最終模型
4. predict.ipynb - 利用上述三個檔案訓練好的模型進行資料預測
## 復現細節
* **檔案執行順序**:
AI_CUP_medical.ipynb &rarr; AI_CUP_acoustic.ipynb &rarr; AI_CUP_second-stage.ipynb &rarr; predict.ipynb
* **說明**:
    * 執行各檔案前，必須先在前三個檔案中的「資料路徑設定」Cell下設定好**病理資料與音訊資料的路徑**以訓練模型，並在predict.ipynb中的「資料路徑設定」設定欲分類的資料集的路徑
    * 訓練過程會自動產生儲存模型參數或路徑的檔案，請勿更動。包含以下檔案:
    1. AI_CUP_medical_model.joblib
    2. accoustic_model(folder)
    3. accoustic_model_path.txt
    4. final_model.joblib
    
 
