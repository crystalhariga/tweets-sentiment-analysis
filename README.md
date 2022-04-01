# What Does the Public Think About ___?
### Background
Let's fill in the blank with Will Smith, Anna Delvey or Climate Change. What do these things have in common? These are trending topics that everyone seem to have an opinion about. But what are people saying about these topics? Are they positive or negative? That's where this tweets dashboard comes into play.

### Project Result
An interactive dashboard that allows you to search for a trending topic and displays:
* a wordcloud showing associated keywords
* an indication of polarity of the tweets (Negative or Positive)

#### Tech Stack
* Python (check requirements.txt for more details about packages)
* JavaScript
* AWS

### Data Collection
Obtained data from Twitter Developer API using Elevated access. Limiting to only 300 tweets per request due to the free version.

### Tweets Cleaning
* Removed "RT", URLs, @usernames, "&amp"

### Text Processing
* Removing Punctuation
* Lowering all cases
* Calculating each tweet's polarity
  * Using TextBlob's polarity function (read [here](https://planspace.org/20150607-textblob_sentiment/) for more information)
* Removing stopwords (filler words, e.g. a, an, in)

### Future Scope
* Combine with other social media posts or articles to back up hypothesis regarding public view towards the topic
* Include top negative tweets, top positive tweets, polarity distribution, word frequency bar charts

### What I learned
* Jupyter Notebook is great for Data Scientists, but not ideal for deploying work
* Consider time and resources while coding (brush up on Big O Notation)
* Only 50 requests every 15 minutes, be prepared to spend hours to experiment and test code

