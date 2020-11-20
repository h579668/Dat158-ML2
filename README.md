<h1>Dat158</h1>
<h4>"Playing the whole game"</h4>
<p>  
Box office prediction. This is a Kaggle competition were we are presented with metadata on over 7.000 past films from The Movie Database to try and predict their overall worldwide box office revenue.
</p>
<p>
Link to the Kaggle competition: https://www.kaggle.com/c/tmdb-box-office-prediction
</p>
<p>
During this project we will use the eight steps from Appendix B:
</p>
<p>
1. Look at the big picture.<br>
2. Get the data.<br>
3. Discover and visualize the data to gain insights.<br>
4. Prepare the data for Machine Learning algorithms.<br>
5. Select a model and train it.<br>
6. Fine-tune your model.<br>
7. Present your solution.<br>
8. Launch, monitor, and maintain your system.
</p>
<p>
 You can find step 2-6 in the notebook.
</p>
<h3> 1. Look at the big picture </h3>
<p>
Here we use supervised learning, since the provided training examples are labeled. The examples will be used learn the machine what it should look for and therafter use it to predict the future.
</p>
<p>
It is both a multiple regression problem, since the data provides multiple features, and a univariate regression problem, since we want to predict one value for a district.
</p>
<h4> Select a Performance Measure </h4>
<p>
Performance Measure gives an idea of how much error the system typically makes in its predictions, with a higher weight for large errors.
</p>
<p>
There are two ways to measure performans: Root Mean Square Error (RMSE) and Mean Absolute Error (MAE). The main difference between these two is that RMSE is more sensitive to outliers than the MAE. The RMSE performs very well and is generally preferred when outliers are exponentially rare.
</p>
<p>
In this project we will use the RMSE as performance measure.
</p>
<p>Her skal det ligge bilde av RMSE</p>
 <p>
X is a matrix containing all the feature values (excluding labels) of all instances in the dataset. <br>
h is your system’s prediction function, also called a hypothesis.<br>
m is the number of instances in the dataset you are measuring the RMSE on.<br>
x^(i) is a vector of all the feature values (excluding the label) of the ith instance in the dataset.<br>
y^(i) is its label (the desired output value for that instance).<br>
RMSE(X,h) is the cost function measured on the set of examples using your hypothesis h.<br>
</p>
<h3>  7. Present your solution. </h3>
<p>
In our project we have followed 8 steps and at the end made a deployment. The focus in this project was to finish a deployment. Therefore we have done the most efficient way to prepare the data. We have for example dropped alot of features that maybe is more important to the revenue than we thought. Anyways we have chosen to focus on the features we found most important: belongs to collection, budget, genres, original language, popularity, release date and runtime. 
</p>
<p>
After testing the data on several models, we chose to use the Forest Regressor. This because it gave us the best result.
</p>
<h3>  8. Launch, monitor, and maintain your system. </h3>
<p>
 Since we have made a deplyment, there is important to update and maintain the model, in order to prevent it from becoming outdated. The data sources should be connected to the system and it should be tested. In the future other features could be more important as well.
</p>
<p>
It would be necessary to write a monitoring code to keeep track of the system performence. It requires human evaluation, because if the predictions are all wrong, then the code need to be checked and possible edited. To make the best possible predictions, it is important to evaluate the input data quality. Later on it would be possible to use feedback from the users in order to update the model, and also online algorithms.
</p>
