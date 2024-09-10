<script>

export default {
    data() {
        return{ 
            icons: [
                {
                    logo: '../../public/img/footer-facebook.png',
                    href: '#',
                },
                {
                    logo: '../../public/img/footer-periscope.png',

                    href: '#',
                },
                {
                    logo: '../../public/img/footer-pinterest.png',
                    href: '#',
                },
                {
                    logo: '../../public/img/footer-twitter.png',
                    href: '#',
                },
                {
                    logo: '../../public/img/footer-youtube.png',
                    href: '#',
                },  
            ],
        }
    },

  methods: {

    }
}
</script>

<template> 

    <div class="row w-100">
        <div class="col-5">
            <button type="button" class="my-btn fw-bold">
                SIGN-UP NOW!
            </button>
        </div>
        <div class="col-7 d-flex align-items-center justify-content-end">
            <div class="follow fw-bold">FOLLOW US</div>
            <div v-for="(icon, index) in icons" key="index">
                <a :href="icon.href"><img class="ms-4" :src="icon.logo" alt=""></a>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');

*{
  font-weight: bold;
  font-family: 'Open Sans';
}


.my-btn{
    color: white;
    padding: 10px;
    background-color: transparent;
    border-radius: 0;
    border: 2px solid #0C7CEC;
}

.follow{
    color: #0C7CEC;
    font-size: 20px;
}

</style>
