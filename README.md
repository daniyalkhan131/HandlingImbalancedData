# HandlingImbalancedData

imbalanced data creates a problem in model making and checking there accuracy like
if out of 100 rows 1 -ve class and other are +ve so if algo always say =ve then 99%
accracy so we need to tackle that.

methods-
1-under sampling majority class
	by only taking number of rows from majority class equal to minority class rows
	but it is not a good way as a lot of data we are discarding
	(worst approach i think)

2-Over sampling minority class by duplication
	by directly duplicating the ,minority class data to make it equal to majority class
	(it might works)

3-Over sampling minority class using SMOTE
	here we generate synthetic examples using KNN algo
	SMOTE-synthetic minority over sampling technique

4-Ensemble method
	here like having 3000 rows of +ve class and 1000 rows of -ve class so we can do like
	take 1000rows from +ve class and -ve class 1000 rows then built a model 1 then
	take next 1000 +ve class rows and with -ve class 1000 rows built model 2 and so on
	and then do majority voting

5-Focal loss
	it will penalize majority samples during loss calc. and give more wight to minority
	class samples
	read this- https://medium.com/analytics-vidhya/how-focal-loss-fixes-the-class-imbalance-problem-in-object-detection-3d2e1c4da8d7#:~:text=Focal%20loss%20is%20very%20useful,is%20simple%20and%20highly%20effective

