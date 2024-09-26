# Extracting Geographic Relations from Social Media Texts
This is the public repository for the data and results on the the "Extracting variations of geographic relations from large social media text data" paper. 

## Data 
The data was collected via the Meltwater twitter (now X) firehose service. 

The search queries we implemented on Meltwater to collect the tweets are as follows, for all 50 states of the United States:

```
(county\_name OR county\_name OR …) AND state\_name
```

For instance, for any tweets that mentioned any counties in the state of New Jersey, our search query was: 

```
(`Atlantic County' OR `Bergen County' OR `Burlington County' OR `Camden County' OR `Cape May County' OR `Cumberland County' OR `Essex County' OR `Gloucester County' OR `Hudson County' OR `Hunterdon County' OR `Mercer County' OR `Middlesex County' OR `Monmouth County' OR `Morris County' OR `Ocean County' OR `Passaic County' OR `Salem County' OR `Somerset County' OR `Sussex County' OR `Union County' OR `Warren County') AND `New Jersey'
```

Per Metlwater and X guideline, a shareable version of the data with the TweetID is [here](https://github.com/yiyunyc2/geographic-relations/blob/3a8abefeec7aa73d5936b5ceef039d84ae24639f/GeoIsa_50states_tweets_ids.csv). 

## Data cleaning and pre-processing 
The data cleaning and pre-processing steps are demonstrated in [this notebook](https://github.com/yiyunyc2/geographic-relations/blob/e828e8f4b154343e27e68463fd4d9a1da947fad1/Geographic_relations_DataCleaning_Preprocessing.ipynb). 

## Results
Results by each model were generated with the following python notebooks. Instructions on how to run the codes are also provided within each notebook. 

- [Heuristics model](https://github.com/yiyunyc2/geographic-relations/blob/b556923d3efa24bb0392e41bef1e9ae016104a1b/GeoIsa_Heuristics_model.ipynb)
  
- [OpenIE](https://github.com/yiyunyc2/geographic-relations/blob/b556923d3efa24bb0392e41bef1e9ae016104a1b/GeoIsa_OpenIE_model.ipynb)
  
- [BERT](https://github.com/yiyunyc2/geographic-relations/blob/b556923d3efa24bb0392e41bef1e9ae016104a1b/GeoIsa_BERT_model.ipynb)
  
- [GPT 3.5](https://github.com/yiyunyc2/geographic-relations/blob/b556923d3efa24bb0392e41bef1e9ae016104a1b/Geo_Isa_GPT3.5_model.ipynb)
  
- [Mistral](https://github.com/yiyunyc2/geographic-relations/blob/b556923d3efa24bb0392e41bef1e9ae016104a1b/GeoIsa_Mistral_model.ipynb) 

## Data analysis 
Analysis of all five models results can be found in [this notebook](https://github.com/yiyunyc2/geographic-relations/blob/8b3c1ed0854d5a47e9fbd1fa1dcac24a171127fe/Geographic_relations_data_analysis.ipynb). 
