<template>
    <v-data-table
      :headers="headers"
      :items="results"
      :items-per-page="5"
      :item-class= "row_classes"
      class="elevation-1"
    >
    </v-data-table>
  </template>


  <script>
export default {
  data() {
    return {
      headers: [
        { text: 'State', value: 'state' },
        { text: 'nb_users', value: 'nb' },
        { text: 'nb_breweries', value: 'nb2' },
        { text: 'nb_users/nb_breweries', value: 'rat' },
      ],
      results: [
        {
          state: 'Rhode Island	',
          nb: 881,
          nb2: 40,
          rat: 22.0,
        },
        {
          state: 'Massachusetts',
          nb: 7332,
          nb2: 333,
          rat: 22.0,
        },
        {
          state: 'New Jersey',
          nb: 4551,
          nb2: 209,
          rat: 21.8,
        },
        {
          state: 'Alabama',
          nb: 1847,
          nb2: 87,
          rat: 21.2,
        },
        {
          state: 'Georgia',
          nb: 3358,
          nb2: 176,
          rat: 19.1,
        },
      ],
    }
  },
}
</script>
