# HFT-ML-Strategy

Replicate well-designed high frequency trading (HFT) strategies built using machine learning and deep learning techniques. Extract trading signals from multi-level orderbook data.

- Orderbook data: SGX FTSE CHINA A50 INDEX Futures (新加坡交易所FTSE中国A50指数期货) tick depth data

- The training pipline:
  <img src="./Graph/pipline.png" width="650">
  

* Feature Extractor

  * Rise Ratio
  
    <img src="./images/bid1ask1.png" width="650">

  * Depth Ratio
  
    <img src="./Graph/depth.png" width="650">
    
    [Note] : [Feature_Selection] (Feature_Selection) 
 
* Learning Model Trainer
  
  *  RandomForestClassifier
  *  ExtraTreesClassifier
  *  AdaBoostClassifier
  *  GradientBoostingClassifier
  *  SVM
  
*  Use best model to predict next 10 seconds

   <img src="./images/CV_result.png" width="650">
   
*  Prediction outcome

   <img src="./Graph/prediction.png" width="650">
   
*  Profit & Loss

   <img src="./images/best_CV_result_all.png" width="650">
   
   [Note] : [Model_Selection] (Model_Selection) 

 

