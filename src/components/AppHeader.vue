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
            <a :href="link.href" @click="toggleLink(index)">
            {{ link.label }}
            <div :class="{ 'active': active === index }"></div>
            </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

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
        color: black;
        &:not(.active):hover{
        color: rgb(83, 83, 83);
        }
      }
    }
  }
}

.active-text{
  color: $DCBlueColor;
}

.active{
  background-color: $DCBlueBg;
  width: 80%;
  height: 4px;
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%);
}

img{
  margin: 30px 0px;
}

</style>
