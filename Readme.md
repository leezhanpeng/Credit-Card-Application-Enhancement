# Setup Instructions
***

## Packages and versions

numpy >= 1.21.1
pandas >= 1.3.1
matplotlib >= 3.4.2
imbalanced-learn >= 0.9.1

## Flow of files

All code files are stored in `Code` folder and all datasets are stored and exported to `Dataset` folder.
In any case where the code files need to import data, file path of `../Dataset/FILENAME.csv` will be used.

- `DataPreprocessing.ipynb` -> For processing of `credit_record.csv` (One-Hot Encoding, Normalisation etc.). Creates `processed_applications.csv`.
- `ScoreGeneration.ipynb` -> For generating of our own scores (y-labels) tagged to each client in `application.csv`. Creates `scores.csv`.

- `LinearRegressionOnScores.ipynb -> To generate model that produces scores via linear regression.
- `NeuralNetworkRegression.ipynb -> To generate model that produces scores via neural network.

- `LogRClassification.ipynb` -> To generate model that classify clients via logistic regression.
- `DecisionTreeClassification.ipynb` -> To generate model that classify clients via decision tree.
- `RandomForestClassification.ipynb` -> To generate model that classify clients via random forest.
- `NeuralNetworkClassification.ipynb` -> To generate model that classify clients via neural network.

### Running file with local machine

Simply run each files in their respective folder.

### Running file on Colab

1) Open the needed ipynb file in Colab.
2) Enter files tab on the left and click on `..`.
3) Create a folder called `Dataset` and add all the csv files into the folder.
4) Run the ipynb file as accordingly.