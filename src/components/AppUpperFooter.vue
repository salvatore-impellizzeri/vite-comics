<script>

export default {
    data() {
        return{ 
            sections: [
                {
                    icon: '../../public/img/buy-comics-digital.comics.png',
                    label: 'DIGITAL COMICS',
                    href: '#',
                },
                {
                    icon: '../../public/img/buy-comics-merchandise.png',
                    label: 'DC MERCHANDISE',
                    href: '#',
                },
                {
                    icon: '../../public/img/buy-comics-shop-locator.png',
                    label: 'SUBSCRIPTION',
                    href: '#'
                },
                {
                    icon: '../../public/img/buy-comics-subscritions.png',
                    label: 'COMIC SHOP LOCATOR',
                    href: '#',
                },
                {
                    icon: '../../public/img/buy-dc-power-visa.svg',
                    label: 'DC POWER VISA',
                    href: '#',
                }
            ],
        }
    },

  methods: {

    }
}
</script>

<template> 

    <div class="bg-upper-footer w-100">
        <div>
            <a :href="section.href" class="d-flex" v-for="(section, index) in sections" key="index">
                <div>
                    <img :src="section.icon" alt="">
                </div>
                <div>
                    {{ label }}
                </div>
            </a>
        </div>
    </div>

    <!-- LOWER FOOTER -->

    <div>
        
    </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

.bg-upper-footer{
    background-color: $DCBlueBg;
}

</style>
