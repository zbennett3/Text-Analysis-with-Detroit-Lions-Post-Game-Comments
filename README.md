# Text Analysis with Detroit Lions Post Game Comments
My goal with this project was to demonstrate text web scraping and to perform text analysis. To do so, I utilized the Reddit API and the Detroit Lions subreddit (r/detroitlions). I accessed the Post Game Comment Thread for the Monday Night Football game against the Raiders on October 30th, 2023. I then pulled in the comments from this thread for text analysis.

For text analysis, I gathered word count, character count, average word length, and more for each comment. I then performed some cleaning by removing punctuation, stopwords, removing rare words, removing common words, and experimenting with TextBlob for spelling correction.

For NLP techniques, I lemmatized and tokenized each comment. I generated term frequency (tf) and then inverse document (idf); I performed sentiment analysis. Afterwards, I utilized the Gensim package to perform topic modelling, where I created an interactive Intertopic Distance Map visualization to explore the emerging topics.

When exploring the visualization, you can quickly see a few themes emerge. You will notice the term "gibbs" being used frequently, which is referring to the Detroit Lions running back Jahmyr Gibbs. He had an amazing performance during this game, 152 yard gained with a touchdown. You will also notice references to "mistakes", "ugly", "turnovers". Despite winning, the Detroit Lions commited 3 turnovers that game, including a fumble and interception (which you will find terms of in the analysis too).

Contents of this collection:

1. reddit_scrape_text_analysis.ipynb: This is the Jupyter Notebook where the text scraping and text analysis is performed.
2. lda_visualization.html: This is the shareable version of the interactive Intertopic Distance Map visualization.

Note:
To access the Reddit API, you will need a client ID, client secret, user agent, username, and password. I used the praw python package to enter my credentials safely for sharing. When running the praw package, it will prompt you to type enter credential needed - pressing the ENTER key each time to confirm it.
