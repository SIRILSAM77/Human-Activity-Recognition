# Human-Activity-Recognition
Human activity Recognition(Classification) is done on data collected using Gyroscope and Accelerometer by using machine learning and deep learning techniques
Description
These days Smartphones have become an integral part of our life. We cannot assume our life without a mobile phone. Since, the advent of Smartphones, a revolution has been created in the mobile communication industry. Smartphones are not just restricted for calling these days. Infact, they are more often used for entertainment purpose.

Smartphone manufacturing companies load Smartphones with various sensors to enhance the user experinece. Two of the such sensors are Accelerometer and Gyroscope. Accelerometer measures acceleration while Gyroscope measures angular velocity.

Here, we will try to use the data provided by accelerometer and gyroscope of Smartphone to classify the activity which a Smartphone user is performing.

Why this is Useful?
These days, in addition to Smartphones, we are also using Smart-Watches like Fitbit or Apple-Watch, which help us to track our health. They monitor our each activity throughout the day check how many calories we have burnt. How many hours have we slept. However, in addition to Accelerometer and Gyroscope, they also use Heart-Rate data to monitor our activity. Since, we only have Smartphone data so just by using Accelerometer and Gyroscope data we will monitor the activity of a person. This software can then be converted into an App which can be downloaded in Smartphone. Hence, a person who has Smartphone can monitor his/her health using this App

Business Problem 
Work-flow is as follows:

Domain experts from the field of Signal Processing collects the data from Accelerometer and Gyroscope of Smartphone. They break up the data in the time window of 2.56 seconds with 50% overlapping i.e., 128 reading

They engineered 561 features from each time window of 2.56 seconds.

By using either human engineered 561 feature data or raw features of 128 reading, our goal is to predict one of the six activities that a Smartphone user is performing at that 2.56 Seconds time window.

Problem Statement
By using either human engineered 561 feature data or raw features of 128 reading, our goal is to predict one of the six activities that a Smartphone user is performing at that 2.56 Seconds time window.

Plan of Action
We will apply classical Machine Learning models on these 561 sized domain expert engineered features.
As we know that LSTM works well on time-series data, so we have decided that we will apply LSTM of Recurrent Neural Networks on 128 sized raw readings that we obtained from accelerometer and gyroscope signals.
Sources 
Data is downloaded from following source: https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones

Constraints:
Some form of interpretability.
There is no low latency requirement here.
Prerequisites
You need to have installed following softwares and libraries in your machine before running this project.

Result:
Using deep learning we improved the Test accuracy to 93.11% and using feature engineering accuracy was improved upto 96% using M.L models
Python 3
Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
Keras
Hyperas
Installing
Python 3: https://www.python.org/downloads/
Anaconda: https://www.anaconda.com/download/
Keras: pip install keras
Hyperas: pip install hyperas
Built With
ipython-notebook - Python Text Editor
sklearn - Machine learning library
seaborn, matplotlib.pyplot, - Visualization libraries
numpy, scipy- number python library
pandas - data handling library
keras - Used for making deep learning models
hyperas - used for tuning hyper-parameters for deep learning models
Authors
Siril Sam
Acknowledgments
Applied AI Course
https://github.com/maxpumperla/hyperas
