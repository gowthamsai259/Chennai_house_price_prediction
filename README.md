# Chennai_house_price_prediction
It's the first time that I have dealt with the large data.
First I have identified that its a numerical or categorical data output, as the data prices are numerical data we can use Linear regression or decision tree algorithms etc

Then the null values in the data were checked and the rows which are having null values were eliminated because it felt like filling the rows with mean values doesnt make sense.
After clearing all the null values the columns were removed which doesnt play a major role in the prediction.
In the cleaning process, as it is pricing data it changes according to the area/location those has to be labeled so the locations which are unique and are less frequent are treated as others.
There were some strings in the columns which were wrongly entered which were corrected by suitable coding.
Finally, in the cleaning process, I have detected the outliers and eliminated them. After the elimination, 4000+ columns were left among 7000+ columns

Then in the Exploratory data analysis, I have found the columns which were correlated in the process I have ended up adding those 2 columns into a single column and removed both the columns(REG_FEE & COMMIS).

Final process in getting the solution for this problem is deploying the model. Necessay libraries are imported and categorial columns are label encoded.
As it is a numerical data, I have used Linear Regression in this model selection, it was split into test and training data as 20 and 80 percent respectively.

R2_score is 77.8 percent which tells that it's a best fit model.
The total process involves 3 simple steps: 1) cleaning the data 2) exploring the data(EDA) 3)suitable model deployment

r2_score and Mean squared error will only be calculated in the linear regression for finding that model is performing well or not.
For categorical output, we will be using accuracy_score, precision, recall, AUCROC to find how better the model is performing.
