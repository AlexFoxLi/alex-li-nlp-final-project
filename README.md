# alex-li-nlp-final-project
This folder is for all the data analyses and codes of the final project. Here are explanations of the files:

"Zhixian_Alex_Li_Final_Project_2024418.ipynb": Code in Python/Google Colab for wrangling the data and doing NLP analysis, results are returned in a csv file

"Assignment Final Statistical Analysis.Rmd": Code in R for doing statistical analysis through ANOVA.

"labeled_data.csv": original data file compiled by Davidson, et al. (2017). Here are some information about its columns - 

  *tweet*: the tweet itself, identified as either containing hate speech or offensive language. It is left in the raw, uncensored form, ready for analysis. 
  
  *count*: the number of CF participants who coded this specific entry (tweet), with a minimum of 3. We can use this to normalize other measures in the data.
  
  *hate_speech*: the number of CF participants who judged the entry (tweet) to be hate speech. Note that it is in raw counts, so we need to normalize it with regard to count.
  
  *offensive_language*: the number of CF participants who judged the entry (tweet) to be offensive. Note that it is in raw counts, so we need to normalize it with regard to count.
  
  *neither*: the number of CF participants who judged the entry (tweet) to be neither offensive nor hate speech. Note that it is in raw counts, so we need to normalize it with regard to count.

"data_final_2024417.csv": data file after NLP processing and used for my statistical analysis. Here are some information about its columns - 

  *neither*: whether or not the tweet is a "neither" tweet - 0 for no and 1 for yes. 
  
  *hate*: whether or not the tweet is a "hate" tweet - 0 for no and 1 for yes. 
  
  *offensive*: whether or not the tweet is an "offensive" tweet - 0 for no and 1 for yes. 
  
  *cw_tweet*: the tweet itself for analysis. 
  
  *hate_score*: semantic similarity score of the tweet with regard to a hate speech corpus. 
  
  *offensive_score*: semantic similarity score of the tweet with regard to an offensive language corpus. 
  
  *neither_score*: semantic similarity score of the tweet with regard to a corpus of non-disturbing tweets. 
  
  *group*: what group does the tweet belong to (hate/offensive/neither). 
  
  *POS*: positive sentiment analysis score (normalized number of positive sentiment words occuring in the tweet). 
  
  *NEG*: negative sentiment analysis score (normalized number of negative sentiment words occuring in the tweet). 
  
  *ANG*: anger emotional analysis score (normalized number of anger emotion words occuring in the tweet). 
  
  *nw*: word count for the tweet.

The purpose of this analysis is to see whether semantic similarity and POS-tagging sentiment analysis could detect differences between hate speech/offensive language/neither categories in tweets collected by Davidson, et al. (2017). 

Reference: Davidson, T., Warmsley, D., Macy, M., & Weber, I. (2017). Automated hate speech detection and the problem of offensive language. Proceedings of the International AAAI Conference on Web and Social Media, 11(1), 512-515. https://doi.org/10.1609/icwsm.v11i1.14955.
