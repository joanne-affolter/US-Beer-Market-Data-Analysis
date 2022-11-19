<template>
  <div>
  <v-card class="mb-6">
    <v-card-title>📍Data pre-processing</v-card-title>
    <v-card-text>
<span color='primary'>Aim:</span> Determine which breweries are the most suitable to be sponsors of major sporting events.<br>
During this part, we pre-process the data to extract the features needed for the project.<br><br>
We first have explored the matched dataset and the other two datasets to determine which one to work on.
Our analyze has shown that the matched dataset did not contain enough data for us to work on it. We will therefore work on the datasets from each website individually.<br><br>
Then we managed to read the ratings file from both websites (RateBeer and BeerAdvocate) and extract the ratings date.
We merged these dates to the beers dataset from each website. We also added the location of each brewery.<br>
One important part of our pre-processing was to filter the data in order to work only with the most popular beers (i.e. with the highest number of ratings) and therefore with the breweries who could be sponsors of such events.
      </v-card-text>
    </v-card>
    <v-card class="mb-6">
    <v-card-title>📍Temporal analysis of the popularity of biggest breweries and the impact of major sporting events on their sales</v-card-title>
    <v-card-text>
      <span color='primary'>Aim:</span> Find a temporal link between the consumption of  beers of the breweries selected in the pre-processing part  and major sporting events
<br><br>
We will look at the evolution over time of the number of ratings and search for some peaks in the data during particular events (Football World Cups, Euro, Super Bowl).
We will group the data in different ways and analyze its temporal evolution to understand how beers' popularity and these events are correlated.
<br><br>
Does a particular style stand out during this period? Are the number of comments on a certain brewery's beers increasing? Is it a sponsor of that event? What about the beer consumption in the **country** hosting such events?<br>
Our main objective is to analyze variation through time, therefore we will use time series methods. We will also perform statistical tests on our data to ensure our conclusions.<br>
We started to analyze the evolution of the top 10 beers and breweries to get a general idea and determine if our project was feasible. We are satisfied with these first results because we do observe peaks in the number of comments on the beers studied during the World Cup period in 2014.
</v-card-text>
</v-card>

<v-card class="mb-6">
    <v-card-title>📍Textual Data Analysis</v-card-title>
    <v-card-text>
      <span color='primary'>Aim:</span>Study whether textual reviews can be used to measure beer popularity<br><br>
Our goal for this part is to analyze the textual reviews and see if we can derive insights from them. In particular, we aim at predicting whether a given review has a positive or negative sentiment. We think that by considering the sentiment associated to a review, we can study the popularity of certain beers better than just by looking at the numerical ratings. The intuition behind this is that a textual review is a richer source of information than a rating between 0 and 5. We hope that by leveraging sentiment analysis, we can encapsulate this additional information and use it as an additional measure for beer popularity. We therefore present a first implementation of a pipeline that:

<v_list>
    <v-list-item>- Extracts textual reviews from the dataset</v-list-item>
    <v-list-item>- Annotates the reviews (positive/negative for later training) using the ratings</v-list-item>
    <v-list-item>- Represents each review in an embedding space</v-list-item>
    <v-list-item>- Trains a classifier on the review embeddings</v-list-item>
    <v-list-item> - Uses the classifier to predict the sentiment of a given review</v-list-item>
    <v-list-item> - Provides a ranking of beer popularity based on sentiment analysis</v-list-item>
      </v_list>
In particular, we will look at the top 10 countries with highest review output and try to find their (semantically) most popular beer. As mentioned above, we have yet no reason to believe that this ranking is more "useful" than a rating-based ranking, we just want to study to what extent these two are different for now.


    </v-card-text>
  </v-card>
</div>
</template>
