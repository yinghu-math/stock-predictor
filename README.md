# stock-predictor

## Introduction 

The application takes two arguments, a valid stock `ticker` (e.g. 'MSFT') and the number of `days` to predict.  

It will return the predicted stock price. 

The prediction model is developed by [Andrew Clark](https://twitter.com/aclarkdata1). 

## Usage instruction 

Use `curl` to access the endpont of the API as follows:  

```bash
curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://44.211.65.246:8000/predict
```

In the example above, the APP will return `7` days prediction of `MSFT`. 

## Project notes

This is a quick project to practice deploying a machine learning model as a RESTful API using [FastAPI](https://fastapi.tiangolo.com/) to AWS EC2, and make it available (i.e., public) to end users. 

Less focus is put on how well the model performs, yet the goal is to get an initial working system quickly into production.

##  

