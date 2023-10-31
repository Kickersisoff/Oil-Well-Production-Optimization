# Oil-Well-Production-Optimization

The primary scope of this project is to forecast the bottom hole pressure (BHP) and production rates for six months(Long time-series forecasting). Input is production data for the well (multiple features).Target is Bottom Hole Pressure (BHP).

🚩: We are Initially utilising ARIMA and then we aim to utilize the combined work by (Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, Wancai Zhang) in Informer forecasting model:Beyond Efficient Transformer for Long Sequence Time-Series Forecasting.

<img src="[https://your-image-url.type](https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/768e16ae-8a7f-4e43-b7ad-0b9ff80b556e)" width="100" height="100">

Figure 1. An example of training dataset

ProbSparse Attention
The self-attention scores form a long-tail distribution, where the "active" queries lie in the "head" scores and "lazy" queries lie in the "tail" area. We designed the ProbSparse Attention to select the "active" queries rather than the "lazy" queries. The ProbSparse Attention with Top-u queries forms a sparse Transformer by the probability distribution. Why not use Top-u keys? The self-attention layer's output is the re-represent of input. It is formulated as a weighted combination of values w.r.t. the score of dot-product pairs. The top queries with full keys encourage a complete re-represent of leading components in the input, and it is equivalent to selecting the "head" scores among all the dot-product pairs. If we choose Top-u keys, the full keys just preserve the trivial sum of values within the "long tail" scores but wreck the leading components' re-represent.

![image](https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/e1fe6725-109e-432f-885b-7e810ebabfa5)

Figure 2. The architecture of Informer model.

Requirements
Python 3.6
matplotlib == 3.1.1
numpy == 1.19.4
pandas == 0.25.1
scikit_learn == 0.21.3
torch == 1.8.0

Figure 4. Univariate forecasting results.


Figure 5. Multivariate forecasting results.
