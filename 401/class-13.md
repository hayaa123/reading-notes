#  How to Run Linear Regression in Python

1- `import sklearn` sk learn is a python pakage containe function for regression, classification, clustering, model selection and dimensionality reduction.

2 - prepeare yor X and Y dimentions forlinear regresion 

for example you have this data 

![boston-data](https://bigdata-madesimple.com/wp-content/uploads/2016/04/RAD.png)

you can set 

Y = boston housing price(also called “target” data in Python)

and

X = all the other features (or independent variables)

like this 

![1](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Skitlearn-linear-model1.png)

```
lm.fit(X, bos.PRICE)

```


# test train split 

we can do petter in spliting the data to x and y like spliting them to testing and training X and y parts 

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Xtrain-and-Xtest.png)

![](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Linear-reg.png)