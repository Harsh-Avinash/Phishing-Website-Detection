# Phishing-Website-Detection
A phishing website is a common social engineering method that mimics trustful uniform resource locators (URLs) and webpages.Phishing websites are created to dupe unsuspecting users into thinking they are on a legitimate site. The criminals will spend a lot of time making the site seem as credible as possible and many sites will appear almost indistinguishable from the real thing.The objective of this project is to train machine learning models and deep neural nets on the dataset created to predict phishing websites. Both phishing and benign URLs of websites are gathered to form a dataset and from them required URL and website content-based features are extracted. The performance level of each model is measures and compared. To find the best machine learning algorithm to detect phishing websites.

## Proposed Methodology
Two python scripts are used for the project, the first to make data ready for our model and the second to Implement and compare the machine Learning algorithms. 

We perform Data preprocessing to make data ready to train for our machine learning models. We make the use of datasets of Benign(legitimate) and malignant URL’s . The new dataset consist of 5000 phishing URLs & 5000 legitimate URLs. By making the use of various User Defined functions we extract the required features. The features we make use of are Domain, Have_IP, Have_At, URL_Length , URL_Depth, Redirection, https, Domain, Tiny_URL,Prefix/Suffix, DNS_Record, Web_Traffic, Domain_Age, Domain_End, iFrame, Mouse_Over, Right_Click, Web_Forwards and Label. 

Thus we make a dataset of only necessary features which is made by combining the Benign and Malignant URL’s. We then export the dataset to a csv file which is used for our machine learning models. We finally extracted 18 features for 10,000 URL which has 5000 phishing & 5000 legitimate URLs. We drop the Domain column and make a new dataset since Domain column won’t help us. We perform the splitting of the data by splitting it into 80 train and 20 test. 

## Result and conclusion 
We make the use of 6Machine Learning Algorithms namely XGboost, Multilayer Perceptrons, Random Forest, Decision Tree, SVM, AutoEncoder. The models are fitted on the training set and the prediction is main using the testing set and test set. We then find the accuracy of both the testing and training data. We plot a confusion matrix to visualize the number of false positives and negatives and the number of true positives and negatives. Finally we compare all the training and testing accuracy and plot it in the form of a graph and Visualize,thus we know that XGboost is the best algorithm for the given data,since it gives us the best accuracy.

![image](https://user-images.githubusercontent.com/64661719/145406126-e05a9570-311e-4a06-bb8a-5e1f61dd1ebd.png)
![image](https://user-images.githubusercontent.com/64661719/145406143-743d76f1-8023-4ea9-8422-34f419c8d356.png)
