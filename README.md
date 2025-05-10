# Country Development Statistics

First install the dependencies:
````shell
python -m venv .venv
source .venv/bin/activate  # for Linux, for Windows replace bin with Scripts
pip install -r requirements.txt
````

To start the Jupyter dashboard locally run

````shell
python -m jupyter notebook
````

The code inside the Jupyter notebook (the .ipynb file) is split up in 3 sections, each one represents a 
question that should be answered with the help of the data from the csv file. The data was taken from the 
webpage of the WorldBank (https://databank.worldbank.org/source/world-development-indicators/preview/on#)
and is the data from 2020 for multiple development indicators for the countries of the world (= the rows in the file).

Initially a Pandas Dataframe is used to load the data from the file, but in a second step is moved to simple
lists to filter out missing data that is represented by `..`.

Each question is tried to answer using a different approach from the course:

- question 1 => Linear Regression
- question 2 => Shaply values
- question 3 => Decision Tree Classifier and Confusion Matrix