<template>
  <v-data-table
    :headers="headers"
    :items="results"
    :items-per-page="5"
    class="elevation-1"
  ></v-data-table>
</template>


<script>
export default {
  data() {
    return {
      headers: [
        { text: 'Diff. between first and last review (years)', value: 'diff' },
        { text: 'Percentage of breweries', value: 'per' },
        { text: 'Average number of ratings per beer', value: 'nb' },
        { text: 'Average rating', value: 'rat' },
      ],
      results: [
        {
          diff: 0,
          per: 6.0,
          nb: 1.3,
          rat: 3.22,
        },
        {
          diff: 1,
          per: 14.0,
          nb: 2.4,
          rat: 3.49,
        },
        {
          diff: 2,
          per: 12.3,
          nb: 3.1,
          rat: 3.49,
        },
        {
          diff: 3,
          per: 10.9,
          nb: 4.2,
          rat: 3.51,
        },
        {
          diff: 4,
          per: 8.2,
          nb: 6.2,
          rat: 3.55,
        },
        {
          diff: 5,
          per: 6.1,
          nb: 7.0,
          rat: 3.5,
        },
        {
          diff: 6,
          per: 3.7,
          nb: 11.3,
          rat: 3.56,
        },
        {
          diff: 7,
          per: 2.4,
          nb: 11.7,
          rat: 3.62,
        },
        {
          diff: 8,
          per: 1.8,
          nb: 11.7,
          rat: 3.49,
        },
        {
          diff: 9,
          per: 1.5,
          nb: 11.8,
          rat: 3.47,
        },
        {
          diff: 10,
          per: 0.8,
          nb: 11.3,
          rat: 3.49,
        },
      ],
    }
  },
}
</script>
