<template>
  <section class="container-fluid py-4">
    <div class="row">
      <div class="col-xl-2">
        <ul class="nav nav-pills flex-column card shadow border-0">
          <li class="nav-item">
            <router-link to="stock-returns" class="nav-link" active-class="active">
              Доходность по акциям
            </router-link>
          </li>
          <li class="nav-item">
            <router-link to="stock-returns" class="nav-link">Stock Returns</router-link>
          </li>
          <li class="nav-item">
            <router-link to="stock-returns" class="nav-link">Stock Returns</router-link>
          </li>
        </ul>
      </div>
      <div class="col-10">
        <div class="card">
          <div class="card-header">
            <h1>Доходность по акциям</h1>
          </div>
          <div class="card-body">
            <router-view/>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FinancialMarkets',
  // computed: {
  //   childRoutes() {
  //
  //   },
  // },
  mounted() {
    // console.log(this.$route);
  },
};
</script>
