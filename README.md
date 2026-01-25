# Chatbot Data Analytics

Analysis of 2.8M Twitter chatbot interactions from customer service conversations.

## Overview

This project analyzes chatbot data to identify communication patterns between customers and support bots. Built during an internship with Open Avenues and Businessolver (Sept-Oct 2022).

## Key Findings

**Volume Growth**
Tweet volume increased by 4 orders of magnitude between Q4 2016 and Q4 2017.

**Top Contributors**
- AmazonHelp: 169,840 tweets (most active bot)
- AppleSupport: 106,860 tweets
- Uber_Support: 56,270 tweets
- 700,000 unique tweeters total

**Temporal Patterns**
- 90% of tweets occurred in Q4 2017
- Weekdays dominated in 2017 (vs Saturdays in 2016)
- Both years showed spikes in early November

**Content Reduction**
Text cleaning removed 40% of original content (590MB → 358MB) by eliminating URLs, punctuation, stop words, and emojis.

## Technologies

- Python
- Pandas (data manipulation)
- Matplotlib (visualization)
- Jupyter Notebook

## Data Structure

Dataset contains 7 columns:
- `tweet_id`: Unique identifier
- `author_id`: Sender address
- `inbound`: Boolean (True = to bot, False = from bot)
- `created_at`: Timestamp
- `text`: Tweet content
- `response_tweet_id`: Original tweet ID
- `in_response_to_tweet_id`: Conversation starter ID

## Analysis Pipeline

1. Load CSV data
2. Clean text (lowercase, remove URLs/punctuation/stop words/emojis)
3. Extract temporal patterns
4. Identify top contributors
5. Compare year-over-year trends
6. Visualize findings

## Author

Steve Eckardt  
