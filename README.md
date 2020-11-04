# Project: Can you recognize the emotion from an image of a face? 
<img src="figs/CE.jpg" alt="Compound Emotions" width="500"/>
(Image source: https://www.pnas.org/content/111/15/E1454)

### [Full Project Description](doc/project3_desc.md)

Term: Fall 2020

+ Team 3
+ Team members
	+ Yue Liang yl4391
	+ Yunuo Ma ym2774
	+ Wannian Lou wl2727
	+ Linh Nguyen lkn2114
	+ Lingjia Zhang lz2720

+ Project summary: In this project, we created a classification engine for facial emotion recognition. We built several models including autoencoder, GBDT, SVM, Weighted SVM, KNN, Random Forest, XGBoost, ResNet50 and Densely Connected Neural Network based on a set of 3,000 facial images (imbalanced with a class ratio of about 4: 1, classified as 0 and 1 respectively) with 2 different types of emotions: compound emotions(classified as 0) versus simple (basic) emotions(classified as 1). Data preprocessing including dealing with imbalanced data (oversampling or generating new data for the class with smaller number of original samples) and images cropping are implemented with different methods for different models. Model evaluation and selection on imbalanced data are implemented. Based on the performance of our models, the best advance model is Densely Connected Neural Network with 0.90 testing accuracy and 0.98 testing AUC, which trained within 3 minutes. Our result is significantly improved comparing to Gradient Boosting Machine(GBM) baseline model with training time around 15 minutes, 0.82 testing accuracy and 0.81 testing AUC. 
	
**Contribution statement**: 

Elise: Ran GBM using original data set, tuned parameters/ performed cross validation, and trained GBM using best parameters to yield baseline; Trained and tested GBM on Balanced data set to see improvement; Tuned parameters/ performed cross validation, and trained other models, including standard SVM on balanced data set, weighted SVM on original data set, and KNN on balanced data set; Formatted file with Markdowns and headers to prep for Main file’s formatting; Wrote installation instructions for Tensorflow; Helped edit Powerpoint presentation formatting and content

Lingjia Zhang: carried out the training using Random Forest and XGBoost and tuned parameters after processing the imbalanced dataset by SMOTE.

Yue Liang:  Preprocessed the imbalanced dataset to create a balanced dataset for the team; Built the advanced model - Densely Connected Neural Network, trained and tested it on the balanced dataset; Built the Autoencoder Model and ran it on the balanced dataset; Built the Logistics Regression, GBDT, GBDT+Logistics Regression; Tuned the parameters of those models using cross validation; Trained and tested them on balanced dataset; Combined the baseline model and the advanced model into the main file and built the prediction codes; Formatted the main files and the notebooks to give more detailed instruction on running the files; Put all models’ metrics together for comparison; Helped edit Powerpoint presentation content and formats.

Yunuo Ma: Built and Implemented ResNet50 model including images cropping, dealing with imbalanced data (oversampling using SMOTE), Normalizing image vectors and convert training and testing labels, trained and tested ResNet50 on balanced dataset; Provided detailed information about model performance and intermediate processing steps. Wrote part of packages installations; Helped plot advanced model; Helped edit Powerpoint presentation content and formats; Formatted and composed README file.

Wannian Lou: Organized all the algorithm and write them into the main file(GBM&DNN) with Yue Liang, made the Powerpoint and cooperate with other teammates. 

Installation instructions:
1.     Download and install Anaconda or the smaller Miniconda.
2.     On Windows open the Start menu and open an Anaconda Command Prompt. On macOS or Linux open a terminal window. Use the default bash shell on macOS or Linux.
3.     Type in pip install --ignore-installed --upgrade tensorflow
4.     Launch Jupyter Notebook from Anaconda Navigator 
 
If that doesn’t work, follow detailed tutorial below: 

https://docs.anaconda.com/anaconda/user-guide/tasks/tensorflow/
1.     Download and install Anaconda or the smaller Miniconda.
2.     On Windows open the Start menu and open an Anaconda Command Prompt. On macOS or Linux open a terminal window. Use the default bash shell on macOS or Linux.
3.     Choose a name for your TensorFlow environment, such as “tf”.
4.     To install the current release of CPU-only TensorFlow, recommended for beginners, type in :
conda create -n tf tensorflow
After it’s done running, type and run the following: 
conda activate tf
Launch Anaconda, in Applications on, select tf. Launch Jupyter notebook from there. Update Anaconda if prompted/ needed.

Install the following packages and others required by the Main file by entering these commands in Anaconda Command Prompt if you don’t already have them:
conda install sklearn: https://scikit-learn.org/stable/install.html
conda install pandas
conda install numpy
conda install matplotlib
conda install scipy
conda install pickle
conda install tensorflow
conda install keras

References: 
Weighted SVM: 
https://machinelearningmastery.com/cost-sensitive-svm-for-imbalanced-classification
Dense NN: 
https://heartbeat.fritz.ai/classification-with-tensorflow-and-dense-neural-networks-8299327a818a
https://digitalcommons.northgeorgia.edu/cgi/viewcontent.cgi?article=1036&context=honors_theses
ResNet50:
https://github.com/keras-team/keras-applications/blob/master/keras_applications/resnet50.py
Past projects: https://github.com/TZstatsADS/Spring2020-Project3-group1

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.


```
proj/
├── data/
├── doc/
├── figs/
├── lib/
└── output/
```

Please see each subfolder for a README file.
