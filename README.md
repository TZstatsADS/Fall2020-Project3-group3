# Project: Can you recognize the emotion from an image of a face? 
<img src="figs/CE.jpg" alt="Compound Emotions" width="500"/>
(Image source: https://www.pnas.org/content/111/15/E1454)

### [Full Project Description](doc/project3_desc.md)

Term: Fall 2020

+ Team 3
+ Team members
	+ Yue Liang yl4391
	+ Yunuo Ma ym2774
	+ Lou Wannian wl2727
	+ Nguyen Linh lkn2114
	+ Zhang Lingjia lz2720

+ Project summary: In this project, we created a classification engine for facial emotion recognition. We built several models including autoencoder, GBDT, SVM, Weighted SVM, KNN, Random Forest, XGBoost, and ResNet50 based on a set of 3,000 facial images (imbalanced with a class ratio of about 4: 1) with 2 different types of emotions: compound emotions versus simple (basic) emotions. Data preprocessing including dealing with imbalanced data (oversampling) and images cropping are implemented with different methods for different models. Model evaluation and selection on imbalanced data are implemented.
	
**Contribution statement**: ([default](doc/a_note_on_contributions.md)) All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.


```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
