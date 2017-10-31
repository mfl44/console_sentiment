# Console Sentiment Analysis

### Overview

- Brief proof of concept sentiment analysis for tweets on the 3 largest consoles (Nintendo Switch, Xbox One, & PS4). All data scraped in Python and all calculations done in Tableau.
- Sample includes the 500 most recent, English-language only tweets that mention each console (static data pulled on 10.31.2017)
- Data scrape and sentiment analysis executed using Python (Tweepy + TextBlob)

### Content

1) Polarity of Tweet by Console
- Measure of the sentiment behind a tweet ranging from -1.00 (very negative) to +1.00 (very positive)
- Each ring represents one tweet and is color coded to show how negative (red) or positive (green) the tweet was

2) Adjusted Polarity of Tweet by Console
- Measure that attempts to take into account the fact that a tweet may not be wholly about the console. This is done by weighting the Polarity using the Subjectivity of the tweet(measure from TextBlob showing how related the tweet is to the console)
- Each ring represents one tweet and is color coded to show how negative (red) or positive (green) the tweet was
[Calculated in Tableau]

3) Number of Tweets by Sentiment
- Table showing the # of tweets each console had per category (Positive, Negative, and Neutral)
- Positive Tweet: Polarity > 0.1
- Negative Tweet: Polarity < -0.1
- Neutral Tweet: 0.1 >= Polarity >= -0.1
[Calculated in Tableau]

4) % of Tweets by Sentiment
- Table showing the % of tweets each console had per category (Positive, Negative, and Neutral)
- Positive Tweet: Polarity > 0.1
- Negative Tweet: Polarity < -0.1
- Neutral Tweet: 0.1 >= Polarity >= -0.1
[Calculated in Tableau]

### Dashboard:

<div class='tableauPlaceholder' id='viz1509419019869' style='position: relative'><noscript><a href='https://public.tableau.com/profile/mike.landron#!/vizhome/Videogame_Console_Sentiment_Analysis/Sentiment_Dashboard'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Vi&#47;Videogame_Console_Sentiment_Analysis&#47;Sentiment_Dashboard&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Videogame_Console_Sentiment_Analysis&#47;Sentiment_Dashboard' /><param name='tabs' value='yes' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Vi&#47;Videogame_Console_Sentiment_Analysis&#47;Sentiment_Dashboard&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>
