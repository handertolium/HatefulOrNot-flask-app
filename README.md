# HatefulOrNot

Sentiment analysis is done on reddit posts dataset, using **tensorflow** and **keras** frameworks. Data consists of over 24000 negative and positive posts.
My model uses single LSTM layer, which gives **87.5%** accuracy. A second part of this repo focuses on integrating saved model into a flask web app called HatefulOrNot.


**Dataset**: [Twitter and Reddit Sentimental analysis Dataset](https://www.kaggle.com/cosmos98/twitter-and-reddit-sentimental-analysis-dataset)

## Web app
App was build with Python framework called Flask and then I used CSS and a little bit of Bootstrap to make web app look better.

## How to set up web app locally
<details><summary>Using cmd and python</summary>

```bash
cd HatefulOrNot
```
```bash
pip install -r requirements.txt
```
```bash

python app.py

```

</details>

<details><summary>Using docker</summary>

```bash
cd HatefulOrNot
```
```bash
docker build -t HatefulOrNot-app
```
```bash
docker run -p 5000:5000 -t -i HatefulOrNot-app:latest 

```
```bash
Go to 127.0.0.1:5000
```
</details>

## How does the web app look?
![Positive result](/img_for_readme/positive_photo.png)
![Hateful result](/img_for_readme/hateful_photo.png)
