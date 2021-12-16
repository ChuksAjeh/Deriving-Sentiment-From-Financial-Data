# Deriving-Sentiment-From-Financial-Data
This is a complete re-work of my Final year Dissertation Project from early-2021. I wanted to address some of the flaws of original project!

## Final-Year-Project - (Original Description)
My Computer Science Final Year Project Investigating correlation between Public Sentiment Data data and Financial Data from the S&amp;P 500

## Overview:

In this project I made a project that looked to understand the relationship between market sentiment data vs market price movement. I created a custom Bi-Directional LSTM model using Tensorflow Library. For comparison I used three other models, Textblob, Flair and Vader. Textblob and Vader are rule-based leixcon type models whilst Flair is another machine learning model like my custom model. The dataset use was DIJA dataset found on Kaggle.

The code runs from main and you have the option to load more of the custom models I saved. These were the resulting models from experiments I had done. if you want more information on these experiments please refer to my paper in the on the repo or contact me for more details.

# Results from the Project:
My model is 50.7% accurate. Not much better than the flip of a coin, but it does work. Textblob proved to be the most accuracte at 51%. Module wise the paper and other related work scored the following:

- Initial Document - Project Proposal 63% - Upper Second Class
- Presentation of Initial Project - 78% - First Class
- Presentation of Final Project - 74% - First Class
- Dissertation - 75% - First Class 

# FLAWS of the Project :

One major flaw is that the data used did not directly feed into the market price movement. The problem with this is that it became an ad-hoc assessment rather than the fundamental basis for the reason a price moved up or down. E.g a Dovish assessment by the head of the Bank of England that causes the FTSE100 to rise in price. The likely cause of this was was my lack of understanding of the kind of information that goes price movements of such markets. The result was was that I tried to place a sentiment at a particular time-slice for the market price. This did not accurately establish a relationship between the market price and my model prediction.

Another flaw was using local machine. I simply did not have enough memory for training which severly hampered the training process of my model and would likely have affected the final accuracy. I intend to use Google Colab next time.

A third flaw is I was comparing machine learning and lexicon models. As much as I hate to agree with the 2nd marker... He is right. They are using different methods from different domains of knowledge to achieve the same goal and so the methods cannot be compared. It's like comparing a bicycle to a car!

Finally the model! Honestly, garbage. Model was an attempt to the faithfully recreate a previous model I had seen, but instead was a mismash of components that largely did not stray from the example model given by Google Tensorflow library. This resulted in a poorly performing model. Yikes! 

## Need for the Rework:

So being frank, a grade is grade! I got a first class and I am most certainly happy! However, in these last few months in industry I have a grown as an engineer, AND now I don't the the threat of a bad grade hanging over my head! So I will take my time and really work on this!

Also this is an opportunity for redesign. I will still use comparison models, but will not use lexicon or rule based models. This is to avoid the mistake I made previously. I will compare it to other ML libraries because why not.

Finally, the idea is to make this a huge repo that will house other ideas such as recession markers. They will likely all be stored on Google Colab so will link to the them there, If I want to make it all fancy with plots and stuff will train the model and save it on colab, and load it locally and visualise the results!

# Other Details and Contact Me!
The link to the previous repo is: https://github.com/ChuksAjeh/Final-Year-Project-

Again any questions about the paper or the models or results please contact me email is on my profile. Or like me if you're too lazy it's chuksajeh@gmail.com

The old code in the repo is commented the code but it's frankly a mess, Hopefully the re-work will serve as 'ready to run' successor! 
