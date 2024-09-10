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
      <div>
        <div class="container-70">
          <AppFooter />
        </div>
      </div>
      <div>
        <div class="container-70">
          <AppFooter />
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
    background-color: $DCBlueBg;
}

.container-70{
  width: 70%;
  margin: auto;
  display: flex;
  align-items: center;
}

</style>

