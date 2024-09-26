# Extracting Geographic Relations from Social Media Texts
This is the public repository for the data and results on the the "Extracting variations of geographic relations from large social media text data" paper. 

## Data 
The data was collected via the Meltwater twitter (now X) firehose service. 

Per Metlwater and X guideline, a shareable version of the data with the TweetID is [here](https://github.com/yiyunyc2/geographic-relations/blob/3a8abefeec7aa73d5936b5ceef039d84ae24639f/GeoIsa_50states_tweets_ids.csv). 

## Data cleaning and pre-processing 
The data cleaning and pre-processing steps are demonstrated in [this notebook](https://github.com/yiyunyc2/geographic-relations/blob/e828e8f4b154343e27e68463fd4d9a1da947fad1/Geographic_relations_DataCleaning_Preprocessing.ipynb). 

## Results
Results by each model were generated with the following python notebooks. Instructions on how to run the codes are also provided within each notebook. 

- Heuristics model
  
- OpenIE
  
- BERT
  
- GPT 3.5
  
- Mistral 

## Data analysis 
Analysis of all five models results can be found in [this notebook](https://github.com/yiyunyc2/geographic-relations/blob/8b3c1ed0854d5a47e9fbd1fa1dcac24a171127fe/Geographic_relations_data_analysis.ipynb). 
