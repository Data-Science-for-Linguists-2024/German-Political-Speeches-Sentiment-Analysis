2/10/24: Working on the project plan! I'm looking more into my data and reviewing Na-rae's comments to get a more solid idea of my project path

# First Progress Report
Link to jnb: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/blob/main/GPS_Sentiment_Analysis.ipynb

Link to data-samples: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/tree/main/data-samples

I loaded one of the xml files into a dataframe and it looked like there are quite a few nan values, but none of them were from columns relevant to my research, so I didnt worry about them. I eventually ended up deleting some of the columns anyway. I thought because there were no NaN values in my needed columns that it would be okay, but apparently the corpus had their own way of marking if they didnt have the info. For 'person' if the speaker was unknown, they put 'k.A.' for 'keine Ahnung' which means 'no idea'. After looking at the urls that these texts came from, I don't think I would be able to figure out who the speaker was, so I decided to drop the rows because it was a very small fraction of the total data. I added a column for what xml file the row came from before merging the files together into one dataframe for ease. I added the political party and gender of each speaker. If you look at my notebook, that section looks a little crazy, but unfortunately, because i was just googling the party information and didn't have an organized list of the speakers' parties, this ended up being the fastest option to adding in the data, since I just copied and pasted the format of the 2 lines of code. I then tokenized the words and sentences, found types, and made bigrams for analysis. 
#### Sharing Plan
I checked the license, and I should be able to distribute/publish all of my data, as long as I give appropriate credit and provide the data's license, so I plan to share all of my data


# Second Progress Report
For my second progress report, I decided to continue with my original JNB and improve upon it rather than make a separate one.

Link to jnb: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/blob/main/GPS_Sentiment_Analysis.ipynb

Link to data-samples: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/tree/main/data-samples

I started by fixing up my notebook and adding better notes throughout to improve the presentation. I made section headers for data and analysis, so things can be more organized for the reader by those sections as things are updated rather than by progress report. I updated the licensing information in my notebook, so it's in line with the data's license. Then, I decided on how to license my own data. 
#### My license 
I decided to maintain the same license as the original dataset I found because I am required to by the original license. It is a Creative Commons Attribution-ShareAlike 4.0 International License. 

I decided to use Ashley's suggestion and add more values for the positions of the speakers. 
Complete your the data acquisition process. I started looking for sentiment analysis tools for German. I found SpaCy which has Sentiws for German. I've installed it and am looking through it to get a better understanding of how to use it for my analysis. This is definitely less than I would like to have done, but unfortunately, it is that time in the semester.

#### Sharing Scheme
I'll be sharing all of my data through my repository because the license the data is under allows any sharing, reproduction or derivation as long as there is proper atribution. This will make it easier for anyone else who might have an interest in using the data to access the data.



# Third Progress Report
Link to jnb: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/blob/main/GPS_Sentiment_Analysis.ipynb

Link to data-samples: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/tree/main/data-samples

Link to README.md: https://github.com/Data-Science-for-Linguists-2024/German-Political-Speeches-Sentiment-Analysis/blob/main/README.md

I spent a good bit of time wrangling with sentiWS because the site I downloaded from was based on an earlier version of spacy, but after I found the updated version, I got to setting up the pipeline. I found the sentiment scores for each speech based on the average score of the tokens. I split the scores into strongly negative, negative, neutral, positive, and strongly positive. I then made a few plots to get a surface level look at the variation of sentiment accross time, political party, office etc. Then, I looked at the statistical significance of the difference between sentiment scores for the speeches from various political parties and offices. Finally, I started the process for topic clustering.  
My data in the notebook is generally in its final form, and the source data files themselves remain unchanged.