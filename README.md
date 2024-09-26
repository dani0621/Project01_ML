# Machine Learning & AI Project 1: NBA Statistics Predictor
## Danielle Li<br />Setepmber 26th, 2024
### Literature Review/Sources
I originally wanted to do a training set with volleyball statistics, but unfortunately, there is not a lot of volleyball statistics previously recorded for me to access. Originally I had wanted to complete a model that could recognize certain actions in volleyball such as hitting, passing, etc. but after doing further research, I found that the project would take more than a month to complete while also needing a lot of resources (lots of storage). There is also very little volleyball games that are recorded consistently and easily accessible, which prompted me to move to NBA statistics. There were many datasets on Kaggle and on the internet in general due to the league's popularity, leading me to find this dataset: [NBA Traditional Boxscores 1997-2024](https://www.kaggle.com/datasets/szymonjwiak/nba-traditional?select=team_traditional.csv). This dataset recorded each NBA game starting in the 1997 season to the 2024 season with the points scored, win/loss (represented by 1 and 0, respectively), blocks, assists, field goals, etc. The multitiude of statistics that was recorded made it favorable and from looking at the data present, I decided that I wanted to create a NBA statistic predictor as there was enough data in csv to hopefully create accurate predictions. I have consistenly watched the NBA in the past couple of years, so I thought it would be fun to do the project on it. In the end, I chose the Kaggle dataset linked earlier for my dataset.

I then looked into current NBA predictors, which led me to this PDF: [Predicting the Outcome of NBA Games](https://digitalcommons.bryant.edu/cgi/viewcontent.cgi?article=1000&context=honors_data_science#:~:text=The%20most%20common%20features%20used,rating%2C%20and%20true%20shooting%20percentage.), which was Matthew Houde's Senior Honors Project for his data science class. Within his paper, he looked at several existing models in order to see if he could improve the efficacy of the models. He ran 6 different models on his testing set in order to see which was the most accurate in its predictions. The results came out to be that the Gaussian Naïve Bayes was the best predictor followed by the Logistic Regression. His research also discussed that Linear Regression was a common model for predicting sports outcomes. The Logistic Regression model to me was the more plausible choice for my NBA Predictor model as I only had a month and very little machine learning background knowledge to complete this project. This led me to watch these Youtube videos: [Python Machine Learning Tutorial (Data Science)](https://www.youtube.com/watch?v=7eh4d6sabA0) and [Linear Regression Analysis](https://www.youtube.com/watch?v=NUXdtN1W1FE), which did provide sample code for my Logistic Regression later on. His work also cited a highly efficient NBA predictor made by Jake Kandell called [NBA Predict](https://github.com/JakeKandell/NBA-Predict/blob/master/createModel.py). Kandell's code for creating the model matched the Youtube videos I had previously watched, leading me to start my project.

####Logistic Regression
Logistc




my problem

why I chose my model for this problem, variables used

why i chose this dataset (include why I chose it and the dataset, include the common columns used, easily formatted)


## how the actual machine learning process went for me
installed libraries, which ones, why (type the actual libraries)

cleaned up data, explain which columns were dropped, excluded, rows dropped

model selection & training, trained for each separate one, adjusted variables used for prediction for each statistics, show example of one?

using the model, implementing it, show the results

# section 3

discuss results, residuals (means squared)/accuracy of the different linear algorithm (show one fo the algorithm's 

how each of the modles could be improved upon, how i couldn't do win probability ina  more equation because i would need the Offensive efficiency: Points scored per 100 possessions. and defensive efficiency: Points allowed per 100 possessions. and other notes stuff abot how it can be improved in the future

if more time, make a comore coplex probability model, find more stats on opponent, etc.


# Section 4

sources, how I used them

