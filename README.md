# Breast Tumour Type Identifier

<h3>Project summary:</h3>

This project is an Identifier of Breast Tumour Type. It is a binary classification project - the tumour can be either Malignant or Benign. I have created a model (using pre-existing models from Scikit-Learn) to detect cancerous tumours. This project analyses the properties of a tumour from digitised images of an FNA (Fine-Needle Aspiration) and predicts whether or not the cell is cancerous based on the properties of the tumour. 

<h3>About the dataset:</h3>

Link to dataset: 
[https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data](https://www.opennn.net/documentation/classification_example.html#DataSet)

<h3>Programs and technologies used:</h3>

-	Google Colab (Hosted Jupyter Notebook Service)
-	Python
-	Different Libraries: NumPy, Pandas, MatPlotLib, Seaborn, Scikit-Learn
-	Models (from Scikit-Learn): Logistic Regression, Decision Tree Classifier, Random Forest Algorithm

<h3>Problem statement:</h3>


Breast Cancer is the most commonly diagnosed cancer amongst women in Australia. According to the National Breast Cancer Foundation, approximately 57 women are diagnosed with Breast Cancer every day, meaning over 20000 women are diagnosed with this cancer every year. 1 in 7 women are diagnosed with Breast Cancer in their lifetime. Currently, approximately one woman under the age of 40 is expected to die each week from breast cancer. In the last 10 years, breast cancer diagnosis has increased by 33%.


Although cell type detection is only a very small part of determining whether or not a tumor is “Malignant” and cancerous, correctly identifying cells within a tumor microenvironment provides oncologists an insight into how a patient’s immune system reacts to the tumor. Machine learning techniques can be used for automatic cell type detection. Such contributions to the classifications of tumors can ensure early diagnosis of breast cancer – meaning that symptomatic breast cancer patients can more likely be treated successfully. 

<h3>Design and features:</h3>

After cleaning, manipulating, exploring and visualizing the data, I split the data into training and testing data sets (75% of the dataset was dedicated to training and 25% of the dataset was dedicated to testing). 

The dependent dataset (Y) contained the diagnosis column – the target values – whether or not the patient has cancer. The independent dataset (X) contained data of the properties of each  tumour (essentially, the data used to achieve the target values).

After scaling the data to ensure all data was of the same magnitude, I trained the 3 models (from Scikit-Learn) on the training data. I found that the Decision Tree Classifier had the highest accuracy of the 3 models (100%) on the training data. I then proceeded to test this model (with the 3 models) on the testing data, using a confusion matrix, and again, found that the Decision Tree Classifier had the highest accuracy of the 3 models (95.3%) on the testing data.

Therefore, the Decision Tree Classifier was the model I decided to employ the classify the tumours (testing data, 25% of the dataset) as Malignant (cancerous) or Benign (non-cancerous).

<h3>Graphs used:</h3>

**Correlation of Properties Heatmap (of first 10 properties):**

<img width="300" alt="Screen Shot 2023-09-26 at 12 10 27 am" src="https://github.com/shree-3143/Breast-Tumour-Type-Identifier/assets/130221650/3dd90951-f098-4ef2-a7c1-8010e4070331">



**Pie Chart of Class Distribution:**

<img width="300" alt="Screen Shot 2023-09-26 at 12 10 01 am" src="https://github.com/shree-3143/Breast-Tumour-Type-Identifier/assets/130221650/390af3b1-17f2-4132-98ed-e4c6c07142bd">



**Count Plot of Class Distribution:**

<img width="300" alt="Screen Shot 2023-09-26 at 12 09 39 am" src="https://github.com/shree-3143/Breast-Tumour-Type-Identifier/assets/130221650/7d13f88e-e8f5-4a59-a657-78e9fb7491aa">


<h3>Final prediction:</h3>

The final step to the project was printing the prediction of the data using the model. As I deduced that the Decision Tree Classifier had the highest testing accuracy, I printed the prediction of the data using this model. Essentially, now we are seeing if the prediction of the independent testing dataset matches the actual dependent testing dataset.

- 1 = Malignant tumour
- 0 = Benign tumour

<img width="1076" alt="Screen Shot 2023-09-26 at 12 22 21 am" src="https://github.com/shree-3143/Breast-Tumour-Type-Identifier/assets/130221650/7d890147-3d81-4ade-ace0-9ef16ec314a5">




Overall, the model is relatively accurate. There are only 7 tumours that the model has identified incorrectly, some being a False-Positive and others being a False-Negative.

In the future, to try and attain closer to 100% accuracy for the predictions of the testing data, I will endeavor to change parameters in the existing models, and experiment with other models.





