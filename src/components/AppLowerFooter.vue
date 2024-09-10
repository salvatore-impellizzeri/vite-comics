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
                <img class="ms-4" :src="icon.logo" alt="">
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

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
