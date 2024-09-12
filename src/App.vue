<script>
import AppHeader from './components/AppHeader.vue';
import AppBody from './components/AppBody.vue';
import AppUpperFooter from './components/AppUpperFooter.vue';
import AppMiddleFooter from './components/AppMiddleFooter.vue';
import AppLowerFooter from './components/AppLowerFooter.vue';
import Card from './components/Card.vue';

export default {
  data() {
    return {

    }
  },

  components: {
    Card,
    AppHeader,
    AppBody,
    AppUpperFooter,
    AppMiddleFooter,
    AppLowerFooter
  }
}
</script>

<template> 

    <!-- HEADER -->

    <div class="bg-header">
      <div class="container-70">
        <AppHeader />
      </div>
      <div class="jumbo">

      </div>
    </div>

    <!-- MAIN -->

    <div class="bg-body d-flex align-items-center position-relative">
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

      <!-- MIDDLE FOOTER -->

      <div class="bg-middle-footer">
        <div class="container-70">
          <AppMiddleFooter />
        </div>
      </div>

      <!-- LOWER FOOTER -->

      <div class="bg-lower-footer">
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

.jumbo{
  height: 500px;
  background-image: url("../../public/img/jumbotron.jpg");
  background-position: top;
  background-size: cover;
}

.bg-body{
  margin: 0;
  padding: 70px 0;
  min-height: 150px;
  background-color: #1C1C1C !important;
}

.bg-upper-footer{
  background-color: #0282F9;
  box-shadow: 0 2px 2px black;
}

.bg-middle-footer{
  background-image: url('../public/img/footer-bg.jpg');
  background-size: cover;
  padding: 70px 0px;
}

.bg-lower-footer{
  position: relative;
  background-color: #303030;
}

.container-70{
  flex-wrap: wrap;
  min-height: 100px;
  width: 70%;
  margin: auto;
  display: flex;
  align-items: center;
}

</style>

