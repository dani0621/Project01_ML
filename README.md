# Machine Learning & AI Project 1: NBA Statistics Predictor
## Danielle Li<br />Setepmber 26th, 2024
### Literature Review/Resources
I originally wanted to do a training set with volleyball statistics, but unfortunately, there is not a lot of volleyball statistics previously recorded for me to access. Originally I had wanted to complete a model that could recognize certain actions in volleyball such as hitting, passing, etc. but after doing further research, I found that the project would take more than a month to complete while also needing a lot of resources (lots of storage). There is also very little volleyball games that are recorded consistently and easily accessible, which prompted me to move to NBA statistics. There were many datasets on Kaggle and on the internet in general due to the league's popularity, leading me to find this dataset: [NBA Traditional Boxscores 1997-2024](https://www.kaggle.com/datasets/szymonjwiak/nba-traditional?select=team_traditional.csv). This dataset recorded each NBA game starting in the 1997 season to the 2024 season with the points scored, win/loss (represented by 1 and 0, respectively), blocks, assists, field goals, etc. The multitiude of statistics that was recorded made it favorable and from looking at the data present, I decided that I wanted to create a NBA statistic predictor as there was enough data in csv to hopefully create accurate predictions. I have consistenly watched the NBA in the past couple of years, so I thought it would be fun to do the project on it. In the end, I chose the Kaggle dataset linked earlier for my dataset.

I then looked into existing NBA predictors, which led me to this paper: [Predicting the Outcome of NBA Games](https://digitalcommons.bryant.edu/cgi/viewcontent.cgi?article=1000&context=honors_data_science#:~:text=The%20most%20common%20features%20used,rating%2C%20and%20true%20shooting%20percentage.), which was Matthew Houde's Senior Honors Project for his data science class. Within his paper, he looked at several existing models in order to see if he could improve the efficacy of the models. He ran 6 different models (Logistic Regression, Random Forest Classifier, K Neighbors Classifier, Support Vector Classifier, Gaussian Naïve Bayes, and XGBoost Classifieron) his testing set in order to see which was the most accurate in its predictions. The results came out to be that the Gaussian Naïve Bayes was the best predictor followed by the Logistic Regression. His research also discussed that Logistic Regression was a common model for predicting sports outcomes. The Linear Regression model to me was the more plausible choice for my NBA Predictor model as I only had a month and very little machine learning background knowledge to complete this project. This led me to watch these Youtube videos: [Python Machine Learning Tutorial (Data Science)](https://www.youtube.com/watch?v=7eh4d6sabA0) and [Machine Learning Tutorial Python - 3: Linear Regression Multiple Variables](https://www.youtube.com/watch?v=J_LnPL3Qg70), which did provide sample code for my Linear Regression model later on. These two videos explained the basics of how Machine Learning worked as well as how it can be implemented within Python. The first video goes through step by step how one would write code if they were to run a python machine learning model, while the second explained the logic behind multiple variables for a Linear Regression. Houde's work also cited a highly efficient NBA predictor made by Jake Kandell called [NBA Predict](https://github.com/JakeKandell/NBA-Predict/blob/master/createModel.py) who used a Linear Regression model for his prediction model which calcalculated the winning percentage of a game between two NBA teams. The popularity of the Linear Regression Model along with the code seeming less complex and doable for a one month project.

I also want to note that ChatGPT and Gemini were both used to debug my code during this process (the exact lines are commented in my code), and ChatGPT was also used to write a few functions that had originally caused bugs in my code. I will go indepth later on about how the two AIs were used.

### Model
I chose to use Colab because it was the service I used when I first learned about machine learning. It was also beneficial that I didn't have to download PyCharm/other services in order to run my code. I started with importing my libraries which I looked off of the youtube videos and Jake Kandell's project. There were more generic imports for data evaluation like numpy, pandas, and math. The libraries I imported from the other sources were from sklearn, which contained tools for machine learning and statistical modeling. I also imported files and drive from google.colab in order to connect my Google Drive account to my Colab. I had previously downloaded the dattaset off Kaggle, which I uploaded to my google drive. Connecting my google drive and colab allowed me to import my data into my Jupyter notebook.
[imports](docs/CONTRIBUTING.md)

I then cleaned my data to preprocess it by deleting the rows that were missing any values and any duplicates. I also created a new dataset which only the games from the 2018-2019 season and onward as data from a larger time period would create a model that was more generalized in its predictions. Data beyond 5 years will start becoming less useful for predictions as the data couldn't reflect current trends. After the seasons before 2019 were taken out, I also created two more functions that I added to the dataset as columns: win percentage and turnover percentage. I obtained the win percentage formula from ChatGPT as the traditional win percentage calculation required point differential, a statistic I didn't have access to. The turnover percentage was found through a quick google search, and I added that column as well to my dataset. Once we had added our new variables, we created a new dataset that only contained the columns/variables we needed for our Linear Algorithms so that are dataset only contained the necessary statistics (dropped unnecessary statistics like game id, type of game, team id, etc.).

For a Linear Regression model, it finds the relationship between a dependent variable and multiple independent variables by creating a linear equation for the data. The equation, essentially, is going to look similar to a linear equation, y=mx+b, except this time, due to the multiple variables, our equation is: y = b + m1x1 + m2x2 + ... + mnxn (different slopes/coefficients for each independent variable which adds up to the value of the dependent variable). I used the Linear Regression model to predict multiple game statistics like Points, Rebounds, Turnovers, Assists, Free Throws Made, Blocks, and Field Goals Made. For each of them, I used different independent variables to predict their statistic because only certain statistics have strong associations with the statistic. For example, for points, I used 










### Problems

why I chose my model for this problem, variables used

why i chose this dataset (include why I chose it and the dataset, include the common columns used, easily formatted)


### how the actual machine learning process went for me
installed libraries, which ones, why (type the actual libraries)

cleaned up data, explain which columns were dropped, excluded, rows dropped

model selection & training, trained for each separate one, adjusted variables used for prediction for each statistics, show example of one?

using the model, implementing it, show the results

### Results

discuss results, residuals (means squared)/accuracy of the different linear algorithm (show one fo the algorithm's 




#### Future Work
how each of the modles could be improved upon, how i couldn't do win probability ina  more equation because i would need the Offensive efficiency: Points scored per 100 possessions. and defensive efficiency: Points allowed per 100 possessions. and other notes stuff abot how it can be improved in the future

if more time, make a comore coplex probability model, find more stats on opponent, etc.

