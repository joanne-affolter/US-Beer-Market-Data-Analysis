


<script>
var data = [
  {
    type: 'choropleth',
    name: 'US states',
    locations: [
      'AL',
      'AK',
      'AZ',
      'AR',
      'CA',
      'CO',
      'CT',
      'DE',
      'FL',
      'GA',
      'HI',
      'ID',
      'IL',
      'IN',
      'IA',
      'KS',
      'KY',
      'LA',
      'ME',
      'MD',
      'MA',
      'MI',
      'MN',
      'MS',
      'MO',
      'MT',
      'NE',
      'NV',
      'NH',
      'NJ',
      'NM',
      'NY',
      'NC',
      'ND',
      'OH',
      'OK',
      'OR',
      'PA',
      'RI',
      'SC',
      'SD',
      'TN',
      'TX',
      'UT',
      'VT',
      'VA',
      'WA',
      'WV',
      'WI',
      'WY',
    ],
    locationmode: 'USA-states',
    scope: 'usa',
    color_continuous_scale: 'Reds',
    z: [
      141, 140, 155, 147, 132, 146, 151, 137, 146, 136, 145, 141, 149, 151, 138, 158, 164, 141, 146, 145, 142, 150, 155,
      160, 156, 161, 147, 164, 150, 152, 155, 167, 145, 146, 151, 154, 161, 145, 155, 150, 151, 162, 172, 169, 170, 151,
      152, 173, 160, 176,
    ],
    zmin: 25,
    zmax: 280,
  },
]

Plotly.newPlot('myDiv', data, layout, config)
</script>



<script>
import Plotly from 'plotly.js-dist/plotly';

export default {
  name: "PlotlyTest",
  data: function() {
    return {
      count: 0,
      data:[{ x: [1,2,3,4], y: [10,15,13,17], type:"scatter" }],
      attr: { displayModeBar: true },
      layout: { title: "My graph :)" }
    };
  },
  methods: {

  },
  mounted() {
    Plotly.plot('plot1', this.data);
  }
