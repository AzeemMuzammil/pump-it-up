# Pump It Up
https://github.com/AzeemMuzammil/pump-it-up/

## Data pre-processing

To explore all of the columns in the data PandasProfiling was used. A few columns in the data contained a substantial number of missing values, in that case, several of the columns were imputed using mean values and elected to delete a few columns right away. Imputing data or filling in missing numbers would have significantly changed the data. Using LabelEncoder, boolean columns were transfered to strings and category columns to integers. Also, for simplicity of use in the later portion, I substituted NaN values with explicit 'n/n' string format. Value counts were used to evaluate columns near similar columns. If the columns were too similar, superior one was kept and the other was discarded. Some of the columns were exactly the same. Later on, when I wanted to create dummy variables for my classification models, this would come in handy. Finally, StandardScaler was used to normalize all of the data columns. Fortunately, the data was relatively clean from there.

## Training

To compare the model performance, I used Random Forest and k-nearest neighbor. Random forest gave better performance than k-nearest neighbor Thus I proceeded with Random Forest. It gave nearly 80% accuracy on the test dataset and 80.96 percent accuracy on the final leaderboard.

## Submission And Ranking

![Screen Shot 2021-09-25 at 01 45 27](https://user-images.githubusercontent.com/33729295/134734611-0e54c2ff-4c40-426c-8c36-4aff1ed79250.png)
