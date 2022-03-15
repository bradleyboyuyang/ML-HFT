# HFT-ML-Strategy

Target: Replicate well-designed high frequency trading (HFT) strategies using machine learning and deep learning techniques. Extract trading signals from multi-level orderbook data.

#### Data
- Futures data: SGX FTSE CHINA A50 INDEX Futures (新加坡交易所FTSE中国A50指数期货) tick depth data

#### Strategy Pipline
<img src="./Graph/pipline.png" width="650">
  
#### Price Series
- Best Bid and Ask Series:

  <img src="./images/best_bid_ask.png" width="750">

#### Feature Engineering & HFT Factors Design
* Depth Ratio and Multi-level Orderbook Imbalance (OBI)
  
  <img src="./Graph/depth.png" width="650">
    
* Rise Ratio on Ask Series
  
  <img src="./images/depth_0915_1130.png" width="650">
  <img src="./images/depth_1300_1600.png" width="650">
    
* Weighted OBI, Depth, and Rise
    
  <img src="./images/rise_1300_1600_w.png" width="650">
 
 #### Model Fitting
- Models
  *  RandomForestClassifier
  *  ExtraTreesClassifier
  *  AdaBoostClassifier
  *  GradientBoostingClassifier
  *  Support Vector Machines
  *  Other classifiers: Multilayer Perceptrons, Softmax, KNN, etc.
   
# Performance Metrics
<img src="./images/CV_result.png" width="650">
<img src="./images/prediction.png" width="650">

   
#### PnL Visualization
<img src="./images/best_CV_result_all.png" width="650">
    

 

