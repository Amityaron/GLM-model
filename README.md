# Generalized Linear Model  <br />
The objective of this project was to construct a Generalized Linear Model (GLM) that establishes a connection between infant mortality and low birth-weight babies. <br />

To initiate the project, we began by reading the file "birthwt.desc.pdf" to gain insights into the data on birth weights. Subsequently, we opened the file "birthwt.data.139.txt," which contained the actual data. <br />

For a comprehensive data analysis, we referred to the file "GLM Birth Weights -pre analysis.edited.pdf," which provided detailed information about the data analysis process. <br />

Throughout the project, the Probit regression link from the following source was utilized: https://en.wikipedia.org/wiki/Probit_model. <br />

In pursuit of our objectives, we employed the following methodologies: <br />

1. Matrix correlation: <br />
2. Automatic Variable Selection Algorithms based on the Akaike Information Criterion (AIC) <br />
<img src="https://github.com/Amityaron/Generalized-linear-model/blob/main/forward-stepwise-algorithm.png" width="40%" height="20%">

3.[Leverage analysis](https://en.wikipedia.org/wiki/Leverage_(statistics)): <br />
   
$$ h_{ii}=(H)_{ii}=x_{i}^T(X^{T}X)^{-1}x_i $$ the $i$ diagonal element of the ortho-projection matrix $H=X(X^TX)^{-1}X^T$

4. Cook's distance examination: <br />

![image](https://github.com/Amityaron/Generalized-linear-model/assets/70226919/7d8e0d61-8aee-4ae3-9b69-3329f2addc6b)

where $p$ is the rank of the model and $\hat{y}_{j(i)}$  is the fitted response value obtained when excluding $i$,and $s^2=\frac{e^Te}{n-p}$ .


6. Exploration of interactions among explanatory variables: <br />
By implementing these methodologies, we aimed to establish a robust GLM model that sheds light on the relationship <br />
between infant mortality and low birth-weight babies. <br />

