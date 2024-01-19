## Machine Learning CS 412 Course Project

Overview of the repository:
First lets gently introduce the main repository

hw_score_predict.ipynb: This Jupyter notebook contains the main analysis and modeling operations of the project. Data preprocessing, feature engineering, model training, and evaluation of results were performed in this file.

scores.csv: It is a data set containing students' homework grades. This data was used in training and testing the model.

chat_history.html: HTML file containing a record of interactions made with ChatGPT. This file was used in the feature engineering process.

So now lets deep into notebook.


Methodology:

For first uploading part we didn't directly upload file as given. We used some techniques like stemming etc. So we want to be sure that our data should be clean as we wanted.
<img width="679" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/e5cb19d1-ab8c-46cd-a2a9-377f4e12793d">

After that for the questions data. We tried to remove unnecesary overloads such as points part. Then we used stemming again.
<img width="1194" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/70afbcfb-7be0-47ad-a527-3b7eda443f89">

Then after that we used vectorizer and TF method. There were a lot of columns and most of them were null, so we want to handle the given columns.
<img width="945" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/543b1eb9-6480-40d5-8947-928d9d93b580">

After that we deleted ChatGPT histories which is given 404.

Then we try different models then finally prepare our results.

Results: 

First we calculated MSE's node by node 

<img width="818" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/a2418f1e-44f7-4727-bdaa-9ea5bce07e8d">

Then we plot the tree. But since it requires a local setup. There is too normal to see it as an error. But we are adding the pdf as image.
<img width="814" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/73ed29e6-9685-4062-9650-260e73c57069">

<img width="1414" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/97007a47-bc73-48e0-9fa1-913d1643215c">

Now time to add the results.

For random forest:
<img width="485" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/53103dad-1b27-4f37-803d-29df38f73377">

For XGBoost:
![image](https://github.com/aydinnntolga/CS412-Project/assets/77833323/671ec4ed-d83a-4ced-9bf3-fce6e3aaac89)

For SVR:
![image](https://github.com/aydinnntolga/CS412-Project/assets/77833323/7b483355-ddff-4388-b834-e98be863dec2)


Comparision of the models: ![image](https://github.com/aydinnntolga/CS412-Project/assets/77833323/d6694654-856f-4b34-aefa-b1db873e6278)

And R^2 scores:
<img width="394" alt="image" src="https://github.com/aydinnntolga/CS412-Project/assets/77833323/c95a88ac-c346-4f70-a532-d23153ea5923">






Team contributions: 

Team
Tolga Aydın
Cenk Şire

Both students made approximately the same contribution. However, in general, their areas of focus were Tolga spending more time on the preparation of Data, while Cenk spent more time on training the model. However, both students looked at the two parts and were not only responsible for their own areas.
