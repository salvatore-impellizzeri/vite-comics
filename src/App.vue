<script>
import AppHeader from './components/AppHeader.vue';
import AppBody from './components/AppBody.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
      message: 'DC Comics'
    }
  },

  components: {
    AppHeader,
    AppBody,
    AppFooter,
  }
}
</script>

<template> 
  <div>
    <div class="container-70">
      <AppHeader />
    </div>
    <div class="container-70">
      <AppBody />
    </div>
    <div class="container-70">
      <AppFooter />
    </div>
  </div> 
</template>

<style lang="scss" scoped>
@use './assets/scss/partials/variables.scss';

.container-70{
  width: 70%;
  margin: auto;
  padding: 30px 0;
  display: flex;
  align-items: center;
}


</style>

