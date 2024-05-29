# Text Analysis with Detroit Lions Post Game Comments
My goal with this project was to demonstrate text web scraping and to perform text analysis. To do so, I utilized the Detroit Lions subreddit (r/detroitlions). I accessed the Post Game Comment Thread for the Monday Night Football game against the Raiders on October 30th, 2023. I then pulled in the comments from this thread for text analysis.

For text analysis, I gathered word count, character count, average word length, and more for each comment. I then performed some cleaning by removing punctuation, stopwords, removing rare words, and experimenting with TextBlob for spelling correction.

For NLP techniques, I lemmatized and tokenized each comment. I generated term frequency (tf) and then inverse document (idf); I performed sentiment analysis. Afterwards, I utilized the Gensim package to perform topic modelling, where I created an interactive LDA visualization to explore the topics. 



