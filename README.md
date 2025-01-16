
# stock_LSTM

This project aims to predict the next day's stock price given past/historical data. Currently, the program predicts the price of TM stock for 12/28/2024. If you want to change the stock/date that is predicted, upload your own history_price.csv file.


## Run Locally

Clone the project

```bash
  git clone https://github.com/anish-c1/stock_LSTM.git
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Train the model and predit the next day's price

```bash
  python LSTM_train.py --data_file history_price.csv --num_epochs 100 --batch_size 32 --checkpoint_path lstm_checkpoint.pth
```


## Environment and Data

Program structure

```bash
C:\Users\anish\PycharmProjects\stock_LSTM
├── LSTM_model.py
├── LSTM_train.py
├── history_price.csv
└── requirements.txt 
```
Environment settings

```bash
pip install -r requirements.txt
```

Data:

The data used in this article is the stock price history of Toyota Motor Corp (NYSE: TM), saved in a CSV file with the following columns: Ticker (copmany ticker), DTYYYYMMDD (date), OpenFixed (open price), HighFixed (high price), LowFixed (low price), CloseFixed (close price), Volume (volume).

