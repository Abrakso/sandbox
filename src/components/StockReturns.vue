<template>
  <div>
    <i class="display-5">
      r<sub>i</sub> = (d + (P<sub>i</sub> - P<sub>0</sub>)) / P<sub>0</sub> &times; 100
    </i>
    <hr>
    <ul>
      <li>r<sub>i</sub> - доходность за i-тый период;</li>
      <li>d - дивидендные выплаты в i-том периоде;<input type="text" v-model="d"></li>
      <li>P<sub>i</sub> - цена акции в момент окончания i-того периода;<input type="text"
                                                                              v-model="Pi"></li>
      <li>P<sub>0</sub> - цена акции в момент начала i-того периода;<input type="text"
                                                                           v-model="P0"></li>
    </ul>
    <h1>result: {{ ri }}</h1>
<!--    <input type="text" v-model="d">-->
<!--    {{ d }}-->
  </div>
</template>

<script>
export default {
  name: 'StockReturns',
  data() {
    return {
      // asd: 'asd',
      d: null,
      Pi: null,
      P0: null,
    };
  },
  computed: {
    ri() {
      return Math.floor((((this.d + (this.Pi - this.P0)) / this.P0)) * 100);
    },
  },
};
</script>
