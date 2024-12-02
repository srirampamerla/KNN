# KNN

we need to calculate KNN using euclidean/Manhattan etc. if data is continuous
(New data point for each feature,Feature values for each column)

If data is in classification.

In O/P we have (Medium and Large)

After calculating Nearest points

if F(a,b)=1 if a=b else 0

F(medium,medium)=1

we have 3 nearest points=(2.23 med, 6.40 large, 6.7 large)

f(medium,medium)+f(medium,large)+f(medium,large)=1+0+0=1

f(large,medium)+f(large,large)+f(large,large)=0+1+1=2.. Highest is 2 we can this as o/p

For regression we need to average all the nearest distance(2.23+6.40+6.7/3)

# Distance Weightned KNN: 

In above example least distance is 2.23 Which is medium but it is predicted as large). To avoid this type misprediction we need to use Distance weighted KNN.

after calculating diatnce we need to do 1/d^2 -> So rank it(nearest neighbourspoints)

For classification: w1*f(medium,medium)+w2*f(medium,large)+w3f(medium,large)=
w1*f(large,medium)+w2*f(large,large)+w3*f(large,large)


For regression:
W1*y1+w2*y2+w3*y3/w1+w2+w3
y1,y2,y3 are the respective target value of weights

![Alt text](https://github.com/srirampamerla/KNN/blob/main/knn1.png?raw=true)

![Alt text](https://github.com/srirampamerla/KNN/blob/main/knn2.png?raw=true)

![Alt text](https://github.com/srirampamerla/KNN/blob/main/knn3.png?raw=true)
