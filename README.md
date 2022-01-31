# Credit_Risk_Analysis

## Analysis Overview
In this project, Python was used to build and evaluate several machine learning models to predict credit risk.  
WThe following procedures were used: 
- Oversampling the data using the **RandomOverSampler** and **SMOTE** algorithms.
- Undersampling the data using the **ClusterCentroids** algorithm.
- Using a combined approach of over- and undersampling using the **SMOTEENN** algorithm.
- Comparing two machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**.  

The goal is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results 

### RandomOverSampler model  
![image](https://user-images.githubusercontent.com/87709841/151722440-d4600ab9-b08e-478e-8491-14926c322474.png)
![image](https://user-images.githubusercontent.com/87709841/151722500-19fe603a-2f42-4ba4-b63a-b6521337f53d.png)
![image](https://user-images.githubusercontent.com/87709841/151722506-a5695180-b01c-40b8-8448-5ea6ee9466a3.png)  

- The balanced accuracy score is 62%.
- The high risk precision is about 1% only with 60% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 60%.

### SMOTE model
![image](https://user-images.githubusercontent.com/87709841/151723703-7871dbf7-0572-40ff-b0d7-e056ee40d266.png)
![image](https://user-images.githubusercontent.com/87709841/151723710-01677a29-78d6-47be-a9de-6aa11f952f46.png)
![image](https://user-images.githubusercontent.com/87709841/151723716-e3a70068-cf66-44f6-a659-8e60cb082293.png)

- The balanced accuracy score is 65%.
- The high risk precision is about 1% only with 66% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 64%.

### ClusterCentroids model
![image](https://user-images.githubusercontent.com/87709841/151723781-dcb0d55f-0911-46de-a848-4238a732e940.png)
![image](https://user-images.githubusercontent.com/87709841/151723786-e320dc3d-2f96-408c-b2fe-9dc0d4dd4d3e.png)
![image](https://user-images.githubusercontent.com/87709841/151723794-6b3e21f7-9d46-41f3-bef5-081f2250239f.png)

- The balanced accuracy score is 53%.
- The high risk precision is about 1% only with 45% sensitivity which makes a F1 of 1% only.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 61%.

### SMOTEENN model
![image](https://user-images.githubusercontent.com/87709841/151723810-7c8b937a-aa9a-485b-a0d6-c043809976c0.png)
![image](https://user-images.githubusercontent.com/87709841/151723815-f7fbe7e2-0683-4483-be9e-a78e0d133ebe.png)
![image](https://user-images.githubusercontent.com/87709841/151723819-defc0ba6-ef36-44e5-ac6c-4629a59727fb.png)

- The balanced accuracy score is 64%.
- The high risk precision is about 1% only with 57% sensitivity which makes a F1 of 2% only.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 70%.

### BalancedRandomForestClassifier model
![image](https://user-images.githubusercontent.com/87709841/151723824-2e3b812c-cae9-4756-906d-72c3e09b40e6.png)
![image](https://user-images.githubusercontent.com/87709841/151723830-72b08809-3c98-4e3e-938a-6549ac17821f.png)
![image](https://user-images.githubusercontent.com/87709841/151723837-633435ac-8ec3-4216-a982-a0887f2c970c.png)

- The balanced accuracy score is 80%.
- The high risk precision is about 4% only with 89% sensitivity which makes a F1 of 7%.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 71%. 

### EasyEnsembleClassifier model
![image](https://user-images.githubusercontent.com/87709841/151723847-eff9b711-065e-4467-94ae-8ba010ead6e6.png)
![image](https://user-images.githubusercontent.com/87709841/151723857-c10d8628-6c71-42d8-8f50-b1df21e7cc17.png)
![image](https://user-images.githubusercontent.com/87709841/151723865-cbc88c7a-4885-49ff-93fa-0f9a5d18ec33.png)

- The balanced accuracy score is 92%.
- The high risk precision is about 9% only with 94% sensitivity which makes a F1 of 16%.
- Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 89%. 

## Summary
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The Ensemble models brought a lot more improvment, especially on the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a recall of 94% so it detects almost all high risk credit. Typically a good balance of recall and precision is desired and it appears that the Easy Ensemble had the best balance of all the models, because of its high accuracy score and good balance of precision and recall scores. The only remaining question would be, is this a level of risk that is acceptable?  I think its a better model, but I'm not sure I would use it, opting instead for a model that could identify at a better level of precision.
