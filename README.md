# Anomaly Detection Algorithms: A Visit  
## Why look at this problem?  
When I was working for my former employer, a digital advertising company in Japan, there were from time to time some anomaly detection tasks assigned to me which I did not feel very involved in such tasks. As I can remember, I just threw all the data into some model like [Gaussian Processes](https://bugra.github.io/work/notes/2014-05-11/robust-regression-and-outlier-detection-via-gaussian-processes/) and high-lighted all the data which are not in the confidence/prediction interval as the output. I did not think much about if I can explain the results but I was wrong. Indeed, feature engineering is important when you are dealing with data, and there are many powerful models that can handle imbalanced data or outliers very well like gaussian processes or boosted trees. However in most cases, those "outliers" do not only concern us in a data engineering way, but also in business sense. Which, requires the analysts to do more research about this specific problem and provides insights about our data.  
Recently I read about a Q&A post on [Zhihu (a Quora-like site in China)](https://www.zhihu.com/question/280696035), the question is "What are the popular anomaly detection algorithms in data mining?". I went through all the answers and found that there are lot of stuff in this field. So I decided to look at this problem by implementing different methods myself. Could be lot of fun :)  
## Some tools/libraries I will be using
- JupyterLab
- pandas / dask