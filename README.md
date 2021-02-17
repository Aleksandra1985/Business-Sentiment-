# Business-Sentiment
We suggest a specific approach of Business Sentiment as an instrument for measuring the emotional component of an IT ticket. This latent information is extracted from the unstructured IT ticket texts with the help of a lexicon-based approach. As standard lexicons do not work well in our context of IT ticket classification, using the state-of-the-art VADER and LDA, we developed a domain specific lexicon. Each of the words is associated with positive, negative or neutral sentiment. In particular, words with valence score greater than 0 are considered to be positive, whereas words with valence score less than 0 are considered to be negative. All other words are considered to have neutral sentiment. For each IT ticket text, we determine the proportion of words with negative, neutral and positive sentiment together with intensifiers (exclamation marks, capitalizations, special characters, date and time).



# STAGE 1. BS lexicon Reading and Stemming
# STAGE 2. Tasks Corpus (2.1.) Reading, Special Preprocessing
#         (2.2.) Special Symbols and UpperCase counting and
#         (2.3.) English language filtering
# STAGE 3. Find words in the Task that match the BS lexicon 
#         (3.1.) Expressions and (3.2.) Keywords. 
#         Count number of matched words and their total Score
# STAGE 4. Writing of Matched words, their Number and total Score in the *.csv file

Excel *.csv file computing:
# STAGE 5. Calculation the Normalized total Score for each Ticket Description
# STAGE 6. Attention Efforts Level identification
