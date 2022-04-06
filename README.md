# HFT-ML-Strategy

In this project, we provide a framework/pipline for high frequency trading using machine/deep learning techniques. More advanced feature engineering (with depth trade and quote data) and models (CNN, LSTM, LightGBM, Attention, AE, TabNet, GNN, or pre-trained models) can be applied in this framework.

### Target
- Extract trading signals from multi-level orderbook data
- Replicate well-designed high frequency trading (HFT) strategies using machine learning and deep learning techniques

### Data
The SGX FTSE CHINA A50 INDEX Futures (新加坡交易所FTSE中国A50指数期货) tick depth data are used.

### Strategy Pipline
<img src="./Graph/pipline.png" width="650">
  
### Orderbook Signals
We use level-3 deep orderbook data to develop trading signals, including **Depth Ratio**, **Rise Ratio**, and **Orderbook Imbalance (OBI)**.

<img src="./Graph/depth.png" width="650"> 
  
However, there are tons of derivatives of potential signals if we have both the trade and quote data, such as:
- volume imbalance signal
- trade imbalance signal
- technical indicators of bid and ask series (RSI, MACD...)
- different weights on different level of orderbook data
- WAP/WPR, weighted average price
- volume imbalance signal
- .....

**There are tons of excellent features to be explored with trade data and depth ordebook data. In the optiver volatility competition, the training data includes both trade and quote/orderbook, and it contains level-2 data. Many insightful feature engineering techniques can be discovered from the top solutions, which can also be applied in this framework.**
  
### Price Series

<img src="./images/best_bid_ask.png" width="750">

### Feature Engineering & HFT Factors Design
- Simple average depth ratio and OBI:

<img src="./images/depth_0915_1130.png" width="750">
<img src="./images/depth_1300_1600.png" width="750">

- Weighted average depth ratio, OBI, and rise ratio:

<img src="./images/rise_1300_1600_w.png" width="750">
 
 ### Model Fitting
- Models:
  *  RandomForestClassifier
  *  ExtraTreesClassifier
  *  AdaBoostClassifier
  *  GradientBoostingClassifier
  *  Support Vector Machines
  *  Other classifiers: Softmax, KNN, MLP, LSTM, etc.

- Hyperparameters:
  * Training window: 30min
  * Test window: 10sec
  * Prediction label: 15min forward
   
### Performance Metrics
- Prediction accuracy:

<img src="./images/prediction.png" width="750">

- Prediction Accuracy Series:
<img src="./images/single_day_accuracy.png" width="800">

- Cross Validation Mean Accuracy:

<img src="./images/CV_result.png" width="800">

- Best Model:

<img src="./images/best_CV_result.png" width="800">

   
### PnL Visualization
<img src="./images/best_CV_result_all.png" width="800">
    

 

