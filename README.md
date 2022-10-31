# Setup Instructions
***

## Packages and versions

- numpy >= 1.21.1
- pandas >= 1.3.1
- matplotlib >= 3.4.2
- imbalanced-learn >= 0.9.1
- keras >= 2.9.0
- scikit-learn >= 1.1.1

## Flow of files

All code files are stored in `Code` folder and all datasets are stored and exported to `Dataset` folder.
In any case where the code files need to import data, file path of `../Dataset/FILENAME.csv` will be used.

- `DataPreprocessing.ipynb` -> For processing of `application.csv` (One-Hot Encoding, Normalisation etc.). Creates `processed_applications.csv`.
- `ScoreGeneration.ipynb` -> For generating of our own scores (y-labels) tagged to each client in `credit_record.csv`. Creates `scores.csv`.

- `LinearRegressionOnScores.ipynb` -> To generate model that produces scores via linear regression.
- `NeuralNetworkRegression.ipynb` -> To generate model that produces scores via neural network.

- `LogRClassification.ipynb` -> To generate model that classify clients via logistic regression.
- `DecisionTreeClassification.ipynb` -> To generate model that classify clients via decision tree.
- `RandomForestClassification.ipynb` -> To generate model that classify clients via random forest.
- `NeuralNetworkClassification.ipynb` -> To generate model that classify clients via neural network.

### Running file with local machine

Simply run each files in their respective folder.

### Running file on Colab

1. Open the needed ipynb file in Colab.
2. Enter files tab on the left and upload all csv files into the folder.
3. Change all load data paths from `../Dataset/` to `/content/`, with the file name at the back.
4. Run the ipynb file as accordingly.