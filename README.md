# X-Sentiment-Analysis-in-Sp-w-Bert

In the file xDataScrapper we scrape tweets in spanish(w/ a designated query) using X's API and we analize their senetiment respective to the query with ChatGPT 3.5. We later clean
up the data and create a file which we can use to finetune a NLP sentiment analysis model.

In the file DataFineTunning we finetune the model bert-base-spanish-wwm-cased with data extracted in the first file using Hugging-Face for the imports and tokenizers and them performing the finetining itself
with Pytorch. The model is then saved locally and we have a final function which implemets the finetunned model.

## Practial Considerations:
The dataset that is included in the repository is very small since it was created using the free version of X's API, for the creation of a meaningfull dataset it is recomended to 
subscribe to the paid version of the service. Keep in mind that both an OpenAI key and an X API bearer token are required to run the first notebook.

The original X data is saved in tweets.csv and the finetunning data set is analsisDeSentimientos_day_month.csv
