# Text Analysis with Detroit Lions Post Game Comments
My goal with this project was to demonstrate text web scraping and to perform text analysis using python. To do so, I utilized the Reddit API and the Detroit Lions subreddit (r/detroitlions). I accessed the Post Game Comment Thread for the Monday Night Football game against the Raiders on October 30th, 2023. I then pulled in the comments from this thread for text analysis.

For text analysis, I gathered word count, character count, average word length, and more for each comment. I then performed some cleaning by removing punctuation, stopwords, removing rare words, removing common words, and experimenting with TextBlob for spelling correction.

For NLP techniques, I lemmatized and tokenized each comment. I generated term frequency (tf) and then inverse document frequency (idf); I performed sentiment analysis. Afterwards, I utilized the Gensim package to perform topic modelling, where I created an interactive Intertopic Distance Map visualization to explore the emerging topics.

When exploring the visualization, you can quickly see a few themes emerge. You will notice the term "gibbs" being used frequently, which is referring to the Detroit Lions running back Jahmyr Gibbs. He had an amazing performance during this game, 152 yard gained with a touchdown. You will also notice references to "mistakes", "ugly", "turnovers". Despite winning, the Detroit Lions committed 3 turnovers that game, including a fumble and interception (which you will find terms of in the analysis too).

Contents of this collection:

1. reddit_scrape_text_analysis.ipynb: This is the Jupyter Notebook where the text scraping and text analysis is performed.
2. lda_visualization.html: This is the shareable version of the interactive Intertopic Distance Map visualization. This can be downloaded and opened in a browser.
3. requirements.txt: This is a text file containing the required python packages needed to run the Jupyter notebook.

Note: To access the Reddit API, you will need a client ID, client secret, user agent, username, and password. I used the praw python package and getpass.getpass() to enter my credentials safely for sharing. When running the praw package, it will prompt you to type each credential needed - pressing the ENTER key each time to confirm it.

Future Work: This collection was to demonstrate web scraping and text analysis in python. For future improvements, I can specialize and further dive into the proper text cleaning methods that the data needs. Each dataset is unique and has unique conditions, I believe the LDA Model can be improved. Additionally, I could scrape multiple post game comment threads to compile a complete season (or playoff run) to improve my dataset size.
