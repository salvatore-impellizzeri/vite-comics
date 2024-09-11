<script>

export default {
    data() {
        return{ 

        }
    },

    props: {
        cardTitle: String,
        cardImg: String
    },

    methods: {

    }
}
</script>

<template> 
    <div>
        <a href="#">
            <div class="container-img">
                <img :src="cardImg" :alt="cardTitle">
            </div>
        </a>
        <h5>
            {{ cardTitle }}
        </h5>
    </div>
</template>

<style lang="scss" scoped>

.container-img{
    height: 266px;

    img{
        object-fit: cover;
        object-position: top;
        width: 100%;
        height: 100%;
    }
}

h5{
    text-transform: uppercase;
    margin: 30px 0px 70px;
    font-weight: 400;
}

</style>
