# Anomaly Detection Algorithms: A Visit  
## Why look at this problem?  
When I was working for my former employer, a digital advertising company in Japan, there were from time to time some anomaly detection tasks assigned to me. Basically I just threw all the data into some model like [Gaussian Processes](https://bugra.github.io/work/notes/2014-05-11/robust-regression-and-outlier-detection-via-gaussian-processes/) and highlighted the data which are not in the confidence/prediction interval as the output. I did not think much about if I can explain the results but there are much more to be explored than I thought. Indeed, feature engineering is important when you are dealing with data, and there are many powerful models that can handle unbalanced data or outliers very well like gaussian processes or boosted trees. However in most cases, those "outliers" do not only concern us in a data engineering way, but also in business sense. Which, requires the analysts to have a good understanding of the algorithm he is using and also the ability to interpret it in a human-readable way.  
Recently I read about a Q&A post on [Zhihu (a Quora-like site in China)](https://www.zhihu.com/question/280696035), the question is "What are the popular anomaly detection algorithms in data mining?". I went through all the answers and found that there are lot of stuff in this field. So I decided to look at this problem by implementing different methods myself. Could be lot of fun :)  

## Some tools/libraries I will be using  
- JupyterLab
- pandas / dask  

## Useful posts and papers  
- [Metrics, Techniques and Tools of Anomaly Detection: A Survey](https://www.cse.wustl.edu/~jain/cse567-17/ftp/mttad/index.html)
- [数据挖掘中常见的「异常检测」算法有哪些？](https://www.zhihu.com/question/280696035)

# Practice: Credit Card Fraud Detection  
This is a kaggle dataset, problem description goes [here](https://www.kaggle.com/mlg-ulb/creditcardfraud/version/3#). Some notes:  
- Binary classification problem
- Use AUC as the performance metric
- Highly unbalanced:  frauds account takes for 0.172% of all transactions

# About the notebooks  
- [Unsupervised Approaches](unsupervised.ipynb)
- [Supervised Approaches: Classification](classification.ipynb)
