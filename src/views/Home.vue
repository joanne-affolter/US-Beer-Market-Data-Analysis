<template>
  <div>
    <v-card class="mb-6">
      <v-card-title>Beer reviews ⚽🍺🏈</v-card-title>
      <v-card-text>Our idea is to analyze the relation between major sporting events (football world-cups, superbowl, etc.) and beer ratings to evaluate the impact of these huge events on beer consumers and breweries' sales. <br>
More specifically we will search if those sporting events affect beers or breweries' popularity, beer consumption and consumers opinion.

First of all, we will look at the most rated beers and most popular breweries to determine if there exists any temporal correlation between some major sporting events and the popularity of the studied beers/breweries.
*For instance, can we observe a peak every 4 years in the consumption of beers from a certain brewery?*

Then, we will analyze the ratings and reviews in a range of one month around the events which have caught our attention in the first part of the project. Our goal is to understand the variation in ratings and reviews between winning and losing countries.<br>
We will analyze the trends depending on the team's results. We will also look for the effect of these events in the textual reviews by leveraging sentiment analysis.

Finally, the whole process will enable us to evaluate how to adapt the sales of breweries depending on the results.
</v-card-text>

    </v-card>

    <v-card>
      <v-card-title>Research Questions ❓</v-card-title>
      <v-card-text>
        <v_list>
<v-list-item>
  Is there a temporal correlation between the ratings dates and major sporting events ?
</v-list-item>
<v-list-item>
Can we observe a difference in consumption between the users of countries that win/lose a match ?
</v-list-item>
<v-list-item>
Do the winning/losing nations drink the same beer when they win/lose ? Does their consumption increase or decrease ?
</v-list-item>
<v-list-item>
Can textual reviews provide an additional metric for beer popularity in relation to sporting events ?
</v-list-item>
<v-list-item>
Do the breweries sponsoring sporting events earn a positive or negative impact from that marketing campaign ?
</v-list-item>
<v-list-item>
Can we tell which beer to sell to each country depending on the results of given sporting event ?
</v-list-item>
        </v_list>
      </v-card-text>
    </v-card>
  </div>
</template>
