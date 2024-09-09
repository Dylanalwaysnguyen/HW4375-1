# HW4375-1

log 
#1
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='adaptive')
R-squared:': 0.6667391162808624
Mean Squared Error: 19.763869557801467

#2
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='adaptive')
R-squared: 0.6658855456906514
Mean Squared Error: 19.814490133534928

#3
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='constant')
R-squared: 0.6662044904246682
Mean Squared Error: 19.79557527605478

#4
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='invscaling')
R-squared: 0.6670392495025671
Mean Squared Error: 19.746070307623835

#5
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='optimal')
R-squared: 0.6455867589813447
Mean Squared Error: 21.018299498220152

#6
sgd = SGDRegressor(max_iter=2000, tol=1e-4, learning_rate='adaptive')
R-squared: 0.6663924668932474
Mean Squared Error: 19.78442742586764

#7
sgd = SGDRegressor(max_iter=2000, tol=1e-5, learning_rate='adaptive')
R-squared: 0.6656436872756875
Mean Squared Error: 19.82883342552725

#8 

sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='adaptive')
R-squared: 0.6657948959251432
Mean Squared Error: 19.81986607241187

#9 
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='invscaling')
R-squared: 0.6683971964840429
Mean Squared Error: 19.66553794298269

#10
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='adaptive')
R-squared: 0.6661561543275798
Mean Squared Error: 19.798441824049036

#11
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='constant')
R-squared: 0.6371619228370962
Mean Squared Error: 21.517930180172932

#12
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='optimal')
R-squared: 0.64216192525375562
Mean Squared Error: 21.414930585174552

#13 
sgd = SGDRegressor(max_iter=1000, tol=1e-2, learning_rate='constant')
R-squared: 0.6542079072096862
Mean Squared Error: 20.50702662658302

#14
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='constant')
R-squared: 0.6635269499517626
Mean Squared Error: 19.954365470846554

#15
sgd = SGDRegressor(max_iter=1000, tol=1e-4, learning_rate='constant')
R-squared: 0.6531175647107685
Mean Squared Error: 20.571688841606424

#16
sgd = SGDRegressor(max_iter=1000, tol=1e-5, learning_rate='constant')
R-squared: 0.6585236428091235
Mean Squared Error: 20.25108409146953


Report: 
I used a heatmap to look at the features to see what was closest to the target value. The primary reason for doing this is to identify which features have the strongest linear relationships with the target variable. Features that show a high positive or negative correlation with the target have much more of possibility to be strong predictors in the regression model. From there on I used those features. Tuning the learning rate and tolerance in SGDRegressor significantly affects model performance. The learning rate controls how fast the model updates its parameters during training. A smaller learning rate allows for more fine-grained adjustments, improving stability but potentially leading to longer training times. and, a larger learning rate speeds up convergence but risks overshooting the optimal solution, resulting in lower accuracy. However it did not change much of the results possible because first, the performance of SGDRegressor is influenced by more than just the learning rate; other aspects, such as data complexity, feature scaling. if the relationship between the features and the target variable is not linear, simply adjusting the learning rate may not lead to better results. A smaller tolerance value forces the model to continue training until it achieves more precise improvements, potentially increasing accuracy but at the cost of more iterations. However the results didn’t change much due to that being the (tol) determines the threshold for stopping the optimization process and if the model's performance improvement between iterations is smaller than this threshold, training halts. So  if the model has already converged to a near-optimal solution or if the data and feature set have inherent limitations and not effecting results that much. 
