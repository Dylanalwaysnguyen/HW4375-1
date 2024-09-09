# HW4375-1

log 
#1
sgd = SGDRegressor(max_iter=1000, tol=1e-3, learning_rate='adaptive')

R-squared:': 0.6667391162808624
Mean Squared Error: 19.763869557801467

#2
sgd = SGDRegressor(max_iter=1000, tol=1e-3, alpha=0.001, learning_rate='adaptive')
R-squared: 0.6658855456906514
Mean Squared Error: 19.814490133534928

#3
sgd = SGDRegressor(max_iter=1000, tol=1e-3, alpha=0.001, learning_rate='constant')
R-squared: 0.6662044904246682
Mean Squared Error: 19.79557527605478

#4
sgd = SGDRegressor(max_iter=1000, tol=1e-3, alpha=0.001, learning_rate='invscaling')
R-squared: 0.6670392495025671
Mean Squared Error: 19.746070307623835

#5

