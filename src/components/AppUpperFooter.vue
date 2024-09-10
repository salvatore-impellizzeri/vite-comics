<script>

export default {
    data() {
        return{ 
            sections: [
                {
                    icon: '../../public/img/buy-comics-digital-comics.png',
                    label: 'DIGITAL COMICS',
                    href: '#',
                },
                {
                    icon: '../../public/img/buy-comics-merchandise.png',
                    label: 'DC MERCHANDISE',
                    href: '#',
                },
                {
                    icon: '../../public/img/buy-comics-subscriptions.png',
                    label: 'SUBSCRIPTION',
                    href: '#'
                },
                {
                    icon: '../../public/img/buy-comics-shop-locator.png',
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

    <div class="w-100">
        <div class="d-flex justify-content-center align-items-center blue-container">
            <a :href="section.href" class="d-flex align-items-center m-4" v-for="(section, index) in sections" key="index">
                <div>
                    <img :src="section.icon" :alt="section.label">
                </div>
                <div class="m-2">
                    {{ section.label }}
                </div>
            </a>
        </div>
    </div>

</template>

<style lang="scss" scoped>

.blue-container{
    padding: 50px 0;
}

a{
    text-decoration: none;
    color: white;
}

img{
    width: 70px;
    height: 70px;
    object-fit: contain;
}

</style>
