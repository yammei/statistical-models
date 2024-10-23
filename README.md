Model Metrics:

```bash
MAE (%): 1.4106491746705319
RMSE (%): 1.6691941227145795
```

Endogenous Variables: Palo Alto Networks (PANW) Closing Price
Exogenous Variables: S&P500 Companies with highest comovement

Environment Setup

```bash
git init
git remote add origin https://github.com/yammei/statistical-models.git
git pull origin main
python3 -m venv .venv
source .venv/bin/activate
pip3 install -r requirements.txt
```

Running the model

```bash
cd scripts
python3 analyze_comovement.py
python3 retrieve_data.py
python3 train_arimax.py
python3 model_inference.py
```

Resources?

https://www.analyticsvidhya.com/blog/2021/11/basic-understanding-of-time-series-modelling-with-auto-arimax/
