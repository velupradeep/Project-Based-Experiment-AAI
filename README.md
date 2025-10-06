<H3>ENTER YOUR NAME: PRADEEP V</H3>
<H3>ENTER YOUR REGISTER NO: 212223240119</H3>
<H3>DATE: 06.10.2025</H3>
<H1 Align="center">Project Based Experiment<H1>
<H3>Objective:<H3>
Type your objective based on the question
<H3>Program:</H3>

  ```

import nltk
from nltk.sentiment import SentimentIntensityAnalyzer

# Download NLTK resources 
nltk.download('vader_lexicon')

# Load the sentiment analyzer
sia = SentimentIntensityAnalyzer()

# Example Facebook data 
facebook_data = [
  "I love the new feature! It's amazing.",
  "The service was terrible. I'm very disappointed.",
  "Great job on the update!",
  "The product quality is poor. I won't be buying again.",
  
]

# Perform sentiment analysis and filter for negative feedback
negative_feedback = []

for message in facebook_data:
  sentiment_score = sia.polarity_scores(message)['compound']
  if sentiment_score < 0:  # Negative sentiment
      negative_feedback.append(message)

# Print the negative feedback
print("Negative Feedback:")
for feedback in negative_feedback:
  print(feedback)


```


<H3>Output:</H3>

<img width="920" height="154" alt="{14D1B43C-1CC1-4772-A720-E34A20BB8D5D}" src="https://github.com/user-attachments/assets/9500ace7-992a-412c-9542-09ce8393cf05" />


<H3>Result:</H3>

A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.

