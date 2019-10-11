# predicting-booking
To predict the booking charges for a cab booking company
## cleaning training set
Initially train set contained only 7 features and after cleaning it and feature engineering they have been increased to 122
## Using Gradient Boosting
It can bee seen that some values are predicted negatively
moreover the accuracy of test set is around 79.65%
![image](https://user-images.githubusercontent.com/52886443/66639828-44034e80-ec35-11e9-956f-a5de8ddae34e.png)
![image](https://user-images.githubusercontent.com/52886443/66635343-a441c280-ec2c-11e9-9be6-3b3883e23042.png)
## Using random Forest
It can be seen that values are well predicted 
And the accuracy on test set comes out to be 91.5%
![image](https://user-images.githubusercontent.com/52886443/66639917-8167dc00-ec35-11e9-9924-3eb9a95977e7.png)
![image](https://user-images.githubusercontent.com/52886443/66635723-701ad180-ec2d-11e9-9445-512bf87c6f78.png)
## Using XG Boosting
Again values are negative as well as having low accuracy of 80.15% on test set
![image](https://user-images.githubusercontent.com/52886443/66640018-b2481100-ec35-11e9-83dd-e67ac9002da3.png)
![image](https://user-images.githubusercontent.com/52886443/66635550-1914fc80-ec2d-11e9-8a89-4a26d71e3082.png)
## Using Decision Tree
Decision Tree shows an anonymous behaviour, it copies train data and gives an r2_score of 100% while fails on test data
where it gives just 86% of r2_score
![image](https://user-images.githubusercontent.com/52886443/66640119-ed4a4480-ec35-11e9-9ed2-eeb65587b721.png)
![image](https://user-images.githubusercontent.com/52886443/66640196-1bc81f80-ec36-11e9-8641-d68e5db5296a.png)
### From the above it can be seen that only Random Forest predicts the booking(fare) well and Decision Tree copies the train well
Now we will be using AdaBoost to optimize the performance of Random Forest and Decision Tree
### ADA_BOOST with DECISION_TREE
![image](https://user-images.githubusercontent.com/52886443/66640811-41095d80-ec37-11e9-9b8e-4da64ab22e8c.png)
![image](https://user-images.githubusercontent.com/52886443/66640921-6b5b1b00-ec37-11e9-9da0-4d8bce27c375.png)
### ADA_BOOST with RANDOM_FOREST
![image](https://user-images.githubusercontent.com/52886443/66641058-9d6c7d00-ec37-11e9-8b8d-a7664e10981b.png)
![image](https://user-images.githubusercontent.com/52886443/66641113-b6752e00-ec37-11e9-9f3d-a1becf61dfb5.png)

### *** FROM THE ABOVE IT CAN BE CONCLUDED THAT ADA_BOOST WITH DECISION_TREE GIVES BEST OPTIMIZATION ***
