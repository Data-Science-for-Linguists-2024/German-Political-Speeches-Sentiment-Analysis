2/10/24: Working on the project plan! I'm looking more into my data and reviewing Na-rae's comments to get a more solid idea of my project path

# First Progress Report
I loaded one of the xml files into a dataframe and it looked like there are quite a few nan values, but none of them were from columns relevant to my research, so I didnt worry about them. I eventually ended up deleting some of the columns anyway. I thought because there were no NaN values in my needed columns that it would be okay, but apparently the corpus had their own way of marking if they didnt have the info. For 'person' if the speaker was unknown, they put 'k.A.' for 'keine Ahnung' which means 'no idea'. After looking at the urls that these texts came from, I don't think I would be able to figure out who the speaker was, so I decided to drop the rows because it was a very small fraction of the total data. I added a column for what xml file the row came from before merging the files together into one dataframe for ease. I added the political party and gender of each speaker. If you look at my notebook, that section looks a little crazy, but unfortunately, because i was just googling the party information and didn't have an organized list of the speakers' parties, this ended up being the fastest option to adding in the data, since I just copied and pasted the format of the 2 lines of code. I then tokenized the words and sentences, found types, and made bigrams for analysis. 
#### Sharing Plan
I checked the license, and I should be able to distribute/publish all of my data, as long as I give appropriate credit and provide the data's license, so I plan to share all of my data





