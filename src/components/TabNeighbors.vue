<template>
  <v-data-table :headers="headers" :items="results" :items-per-page="6" :item-class="row_classes" class="elevation-1">
    <template v-slot:item.ta="{ item }">
      <v-chip :color="getColor(item.ta)" dark>
        {{ item.name }}
      </v-chip>
    </template>
  </v-data-table>
</template>

<script>
export default {
  data() {
    return {
      headers: [
        { text: 'Name', value: 'name' },
        { text: 'Appearance', value: 'ap' },
        { text: 'Aroma', value: 'ar' },
        { text: 'Palate', value: 'pa' },
        { text: 'Taste', value: 'ta' },
      ],
      results: [
        {
          name: 'Our Beer',
          ap: 3.0,
          ar: 2.0,
          pa: 4.5,
          ta: 0.5,
        },
        {
          name: 'Founders India Pale Ale',
          ap: 3.0,
          ar: 3.0,
          pa: 4.33,
          ta: 4.0,
        },
        {
          name: 'Williamsburg Irish Stout',
          ap: 3.0,
          ar: 2.5,
          pa: 5.0,
          ta: 4.5,
        },
        {
          name: 'Blue & Gray Bormans Belgian Ale	',
          ap: 2.66,
          ar: 2.76,
          pa: 4.9,
          ta: 4.86,
        },
        {
          name: 'Blue & Gray Chocolate Raspberry Stout',
          ap: 3.66,
          ar: 2.72,
          pa: 5.0,
          ta: 4.89,
        },
        {
          name: 'Williamsburg Colonial Mild	',
          ap: 3.0,
          ar: 2.0,
          pa: 5.0,
          ta: 5.0,
        },
      ],
    }
  },
  methods: {
    getColor(ta) {
      if (ta == 0.5) return 'primary'
    },
  },
}
</script>
