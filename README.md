# Data-Driven Long Sequence Forecasting for Oil well Production Optimization

The primary scope of this project is to forecast the bottom hole pressure (BHP) and production rates for six months(Long time-series forecasting). Input is production data for the well (multiple features).Target is Bottom Hole Pressure(BHP), feature Y in the below dataset.

🚩: We are Initially utilising ARIMA and then we aim to utilize the combined work by (Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, Wancai Zhang) in Informer forecasting model:Beyond Efficient Transformer for Long Sequence Time-Series Forecasting.


<p align="center">
<br><br>
<img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/768e16ae-8a7f-4e43-b7ad-0b9ff80b556e" width="600" height="200">
<br><br>
<b>Figure 1.</b> An example of training dataset
</p>


<p align="center">
<br><br>
  <img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/6b4fd649-c8f7-4a32-b24f-a89bb1a84490" width="500" height="300">
<br><br>
<b>Figure 2.</b> Line plot for Target Variable
</p>

#### Informer Model
Informer is an upgraded version of the Transformer model that maintains a larger prediction capacity while being more efficient in terms of architecture, memory usage, and computation. There are several severe issues with Transformer that prevent it from being directly applicable to LSTF (Long sequence Time series forecasting), including quadratic time complexity, high memory usage, and inherent limitation of the encoder-decoder architecture.

<p align="center">
<br><br>
  <img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/e1fe6725-109e-432f-885b-7e810ebabfa5" width="400" height="300">
<br><br>
<b>Figure 3.</b> The architecture of Informer model.
</p>

Requirements
* Python 3.6
* matplotlib == 3.1.1
* numpy == 1.19.4
* pandas == 0.25.1
* scikit_learn == 0.21.3
* torch == 1.8.0

#### Result

<p align="center">
<br><br>
  <img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/5768c826-e927-4b0d-ae85-899cc160da43" width="600" height="300">
<br><br>
<b>Figure 4.</b> Multivariate forecasting results (for 96 days).
</p>

🚩: Find the `Research Report` here - [Link](https://drive.google.com/file/d/1fwwCZzIIfk6Hiip40Z6bgMQQZSp9eS_J/view?usp=sharing)
