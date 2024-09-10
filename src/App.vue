<script>
import AppHeader from './components/AppHeader.vue';
import AppBody from './components/AppBody.vue';
import AppUpperFooter from './components/AppUpperFooter.vue';
import AppLowerFooter from './components/AppLowerFooter.vue';

export default {
  data() {
    return {

    }
  },

  components: {
    AppHeader,
    AppBody,
    AppUpperFooter,
    AppLowerFooter,
  }
}
</script>

<template> 

    <!-- HEADER -->

    <div class="bg-header">
      <div class="container-70">
        <AppHeader />
      </div>
    </div>

    <!-- MAIN -->

    <div class="bg-body d-flex align-items-center">
      <div class="container-70">
        <AppBody />
      </div>
    </div>

    <!-- FOOTER -->

    <div>

      <!-- UPPER FOOTER -->

      <div class="bg-upper-footer">
        <div class="container-70">
          <AppUpperFooter />
        </div>
      </div>

      <!-- LOWER FOOTER -->

      <div>
        <div class="container-70">
          <AppLowerFooter />
        </div>
      </div>

    </div>

</template>

<style lang="scss" scoped>

.bg-header{
  background-color: white;
}

.bg-body{
  margin: 0;
  min-height: 150px;
  background-color: #1C1C1C !important;
}

.bg-upper-footer{
    background-color: #0282F9;
}

.container-70{
  width: 70%;
  margin: auto;
  display: flex;
  align-items: center;
}

</style>

