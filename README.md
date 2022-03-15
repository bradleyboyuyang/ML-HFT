# HFT-ML-Strategy

Target: Replicate well-designed high frequency trading (HFT) strategies using machine learning and deep learning techniques. Extract trading signals from multi-level orderbook data.

#### Data
SGX FTSE CHINA A50 INDEX Futures (新加坡交易所FTSE中国A50指数期货) tick depth data

#### Strategy Pipline
<img src="./Graph/pipline.png" width="650">
  
#### Orderbook Signals
We use level-3 deep orderbook data to develop trading signals, including **Depth Ratio**, **Rise Ratio**, and **Orderbook Imbalance (OBI)**.

<img src="./Graph/depth.png" width="650"> 
  
#### Price Series

<img src="./images/best_bid_ask.png" width="750">

#### Feature Engineering & HFT Factors Design
- Simple average depth ratio and OBI:

<img src="./images/depth_0915_1130.png" width="800">
<img src="./images/depth_1300_1600.png" width="800">
- Weighted average depth ratio, OBI, and rise ratio:

<img src="./images/rise_1300_1600_w.png" width="800">
 
 #### Model Fitting
- Models
  *  RandomForestClassifier
  *  ExtraTreesClassifier
  *  AdaBoostClassifier
  *  GradientBoostingClassifier
  *  Support Vector Machines
  *  Other classifiers: Multilayer Perceptrons, Softmax, KNN, etc.
   
#### Performance Metrics
- Prediction accuracy:

<img src="./images/prediction.png" width="800">

- Prediction Accuracy Series:
<img src="./images/single_day_accuracy.png" width="800">

- Cross Validation Mean Accuracy:
- 
<img src="./images/CV_result.png" width="800">

- Best Model:

<img src="./images/best_CV_result.png" width="800">

   
#### PnL Visualization
<img src="./images/best_CV_result_all.png" width="800">
    

 

