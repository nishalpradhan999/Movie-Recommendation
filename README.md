Movie-Recommendation
=============================
### Introduction 
Movie Recommendation Engine Based on Python which uses the __PCS(Pearson Correlation Similarity) Measure__ to solve for the *closest in likings* users to estimate ratings given to movies by a user which is a __Collabrative Filtering Methodology__.The Engine then uses __K-Means clustering__ to cluster movies of similar genre into groups for boosting the performance and accuracy of predictions. Also made a basic terminal app which asks the user to rate certain movies and the recommends genre based on ratings as well as show to closest users thus predicting age,sex etc. 
### Dataset and Results
The datatset used for the training and testing of the engine is the __MovieLens100K dataset__ . The schema of the dataset can be read about [here](http://files.grouplens.org/datasets/movielens/ml-100k-README.txt) or in the */data* repo . In brief the dataset has 100,000 user ratings (valued between 1-5) for 943 users across 1682 movies . Along with that essential features of users like age,sex,occupation and zipcode as well as essential features of movies like genre,year etc are provied.</br>
The Engine accuracy will be measured using __Mean squared error__ evaluation between predicted rating and ground truth rating which can be checked [here](https://github.com/AadityaJ/Movie-Recommendation/blob/master/Recommend.ipynb#Result) which of around __1.256__.Besides this PCS generated a utility matrix heatmap ![given here](http://www.aadityajamuar.net/selfplots/pcs.png) </br> 
as well as a user vs ratings heatmap </br>
![generated here](http://www.aadityajamuar.net/selfplots/ratings.png)

### File system
The code to replicate the tests on MovieLens dataset is given in Main.py . Run using 

```
$ python Main.py
```
Although all the results are saved in *movielens.ipynb* along with the results and the plots.The data can be found in the */data* repo.Also to run the terminal app:
```
$ python gui.py
```
### Terminal App
The Terminal App uses the concept of closest users to current user based on 10 random movies rated by the (current)user upon which he or she is recommended 5 genre as well as shown closest users.
</br>
An example would be like ![this](http://www.aadityajamuar.net/selfplots/Terminal_Reccomend.png)
### Downloads and Contribution 
To clone the repo 
```
$ git clone https://github.com/AadityaJ/Movie-Recommendation
```
Feel free to Fork the code.
To send a Pull Request please contact :
* Aaditya Jamuar ([@AadityaJ](https://github.com/AadityaJ))
