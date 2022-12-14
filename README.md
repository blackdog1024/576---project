# 576---project

## Data preprocessing
data url: https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification/data

only download train.csv and put it in ./data/train.csv

run `python dataclean.py`  to generate balanced data after cleaning 

[cleaned data without balanced]   ./data/new_train.csv          

[cleaned and balanced data]  ./data/balanced_train.csv          



## The latest version: three_models.py

run `python three_models.py`

RNN, LSTM, GRU, LSTM with GloVe, GRU with GloVe

### Download GloVe 
```
!wget http://nlp.stanford.edu/data/glove.6B.zip

!unzip glove.6B.zip

!ls -lat
```

### Select models
 
use `MODEL = 'GRU'`  to select a model (RNN/LSTM/GRU)

set `PRE_TRAIN = True` if using GloVe

Data path: ./data/balanced_train.csv

GloVe path : ./data/glove.6B.50d.txt

