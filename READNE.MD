# Overview

Analyze financial data, focu son VaR. Cliassical and "new" Neural Network approach.

# Data

Data loaded from ALPHAVANTAGE. Docu her: [https://www.alphavantage.co/documentation/](https://www.alphavantage.co/documentation/)
To persist data, postgres db is used. Free endpoint only allows for approx 25 calls per day. PG set up with

```bash
docker run -d  --name pg_finance -e POSTGRES_USER=myuser -e POSTGRES_PASSWORD=mypassword -e POSTGRES_DB=finance_db -p 7005:5432 postgres:latest
```

# Setup

I use python 3.11.9.

Setup env:

```bash
pip install -r requirements.txt
```
