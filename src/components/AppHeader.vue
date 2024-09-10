<script>

export default {
  data() {
    return {
      links: [
        {
          label:"CHARACTERS",
          href:"#",
        },
        {
          label:"COMICS",
          href:"#",
        },
        {
          label:"MOVIES",
          href:"#",
        },
        {
          label:"TV",
          href:"#",
        },
        {
          label:"GAMES",
          href:"#",
        },
        {
          label:"COLLECTIBLES",
          href:"#",
        },
        {
          label:"VIDEOS",
          href:"#",
        },
        {
          label:"FANS",
          href:"#",
        },
        {
          label:"NEWS",
          href:"#",
        },
        {
          label:"SHOP",
          href:"#",
        }
      ],
      active: 1,
    }
  },

  methods: {
    toggleLink(index){
      this.active = index;
    }
  }
}
</script>

<template> 
  <div class="row w-100">
    <div class="col-4">
      <img src="../../public/img/dc-logo.png" alt="">
    </div>

    <!-- NAV BAR -->

    <nav class="col-8">
      <ul>
        <li v-for="(link, index) in links" key="index">
            <a class="sans" :href="link.href" @click="toggleLink(index)" :class="{ 'active-text' : active === index }">
            {{ link.label }}
            <div :class="{ 'active': active === index }"></div>
            </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');

*{
  font-weight: bold;
  font-family: 'Open Sans';
}

.col-8{
  display: flex;
  align-items: center;

  ul{
    height: 100%;
    width: 100%;
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: space-between;

    li{
      position: relative;
      display: flex;
      align-items: center;

      a{
        text-decoration: none;
        color: rgba(0, 0, 0, 0.7);
        &:not(.active):hover{
        color: black;
        }
      }
    }
  }
}

.active-text{
  color: #0282F9 !important;
  transition: 0.2s ease-in-out;
}

.active{
  background-color: #0282F9;
  width: 100%;
  height: 4px;
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%);
  transition: 0.2s ease-in-out;
}

img{
  margin: 30px 0px;
}

</style>
