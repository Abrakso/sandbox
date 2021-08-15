<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <router-link to="/" class="navbar-brand p-0">
        <logo class="header-logo"/>
      </router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
              data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup"
              aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <router-link to="fin-market" class="nav-link">Financial Markets</router-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import Logo from '@/components/svg/Logo.vue';

export default {
  name: 'HeaderComponent',
  components: {
    Logo,
  },
};
</script>

<style lang="scss">
.header {
  &-logo {
    width: 40px;
    height: auto;
  }
}
</style>
