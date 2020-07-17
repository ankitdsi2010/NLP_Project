# Parts of Speech Tagging  

In this, I used web scraping to obtain the data for which I used the BeautifulSoup Library.

After obtaining the data, I cleaned the data by
* removing special characters
* removing html tags
* stemming the words
* lemmatizing the words
* removing stop words
* converting text to lower case  

After this, I applied POS tagging to the text by using Spacy library as it gives a rather accurate result for this purpose than NLTK.

Then I created a table as the output demanded having Part of Speech, Words and Word Count as columns.
