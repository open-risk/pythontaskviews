## Python Task Views: Regression Methods

### Scope, Organization, Caveats
The scope aims to cover typical regression methods, not edge cases. Regressions in relation to timeseries data are to be covered in the [Econometrics](Econometrics.md) Task View. The entries are grouped together roughly by similarity of purpose (use case) and problem context but there can be obviously substantial overlap

When there is no package identified that appears reasonably stable / mature the corresponding slot is simply empty

Listing here does not imply any sort of assurance about the quality of algorithms, the degree of testing etc. Always test packages and functionalities to a degree proportional to the significance, requirements and sensitivity of your data science task.

### Packages offering regression methods functionality

* The first column indicates the specific method and / or functionality along with a documentation link where the mathematics of the method is documented in detail
* The second column has links to functionality offered by the lower level packages scipy/numpy/pandas (where available) 
* The third column has links to the standard statistical packages (scikit-learn and statsmodels)
* The fourth column has links to deep learning packages (where regressions methods are already released)
* The fifth column is reserved for more specialized projects

| Functionality / Documentation | Scipy/Numpy/Pandas | Scikit-learn/Statsmodels  | Pytorch/TensorFlow |  Other |
|-------------------------------| ------------ |-------------------------- | ----- | -------- |
| [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression)  | [scipy.stats.linregress](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.stats.linregress.html), [numpy.linalg.lstsq](https://docs.scipy.org/doc/numpy/reference/generated/numpy.linalg.lstsq.html)| Placeholder | Placeholder| Scipy/Numpy offer low level least squares routines |
| Generalized Liner Regression  | Placeholder |  Placeholder     | Placeholder  | Placeholder  |
| Fractional Response Regression  | Placeholder |  Placeholder     | Placeholder  | Placeholder  |
| Beta / Inflated Beta Regression  | Placeholder |  Placeholder           | Placeholder | Placeholder  |
| Polynomial Regression  | Placeholder |  Placeholder           | Placeholder           | Placeholder  |
| [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression)  | Placeholder | [Statsmodels.logit](http://www.statsmodels.org/dev/generated/statsmodels.discrete.discrete_model.Logit.html), [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) |  Placeholder           | Placeholder  |
| Probit Regression  | Placeholder |  Placeholder           | Placeholder           | Placeholder  |
| Multinomial Regression  | Placeholder |  Placeholder           | Placeholder           | Placeholder  |
| Ordinal Regression  | Placeholder |  Placeholder           | Placeholder           | Placeholder  |
| [Stepwise Regression](https://en.wikipedia.org/wiki/Stepwise_regression) | Placeholder | Placeholder |Placeholder | Placeholder |
| [Ridge Regression (Tikhonov Regularization)](https://en.wikipedia.org/wiki/Tikhonov_regularization) | Placeholder | [sklearn.linear_model.Ridge](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html) | Placeholder | Linear least squares (Various Solvers) with L2 Regularization |
| [Lasso Regression](https://en.wikipedia.org/wiki/Lasso_(statistics))  | Placeholder |  [sklearn.linear_model.Lasso](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Lasso.html)         | Placeholder           |Coordinate descent with L1 Regularization  |
| [Elastic Net Regression](https://en.wikipedia.org/wiki/Elastic_net_regularization) | Placeholder |  [sklearn.linear_model.ElasticNet](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ElasticNet.html)        | Placeholder           | Coordinate descent with L1 + L2 Regularization  |
| Bayesian linear regression | Placeholder |            | Placeholder           | Placeholder  |
| [Segmented regression](https://en.wikipedia.org/wiki/Segmented_regression) | Placeholder |  Placeholder | Placeholder           | Placeholder  |
| [Robust regression](https://en.wikipedia.org/wiki/Robust_regression) | Placeholder | [statsmodels.robust](https://www.statsmodels.org/devel/generated/statsmodels.robust.robust_linear_model.RLM.html#statsmodels.robust.robust_linear_model.RLM) | Placeholder | Placeholder  |


## Notes
* Tensorflow modules reference 2.0 only

