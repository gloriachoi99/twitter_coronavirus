# Coronavirus analysis

This repo analyzes the activity of coronavirus hashtags on twitter. This was a homework assignment for the CS046 class at Claremont McKenna College in Spring 2020. I was tasked with scanning all geotagged tweets sent after November 2019 to monitor the spread of the coronavirus on social media.

I edited the map.py file in the src directory to show, in addition to which language a tweet was written in, where the tweet came from. I used Python dictionaries to account for tweets that did not come from a specific country (e.g. tweets sent over international waters) as well as tweets that were geotagged from a specific country. 

I organized my results by hashtag in the 'viz' directory. There are 17 hashtags related to the coronavirus in English, Japanese, Chinese, and Korean. I globbed the output files listing the countries ('unknown' for tweets with unspecified countries) and languages of the tweets in reduced.country and reduced.lang files respectively.

To visualize the outputs of each of these files, enter the following command:

$ ./src/visualize.py --input_path=reduced.TYPE --key='HASHTAG'

and replace [TYPE] with [lang] or [country] and [HASHTAG] with the desired hashtag.    
