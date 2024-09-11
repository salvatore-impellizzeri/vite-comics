<script>

export default {
    data() {
        return{ 
            sections: [
                {
                    title: 'DC COMICS',
                    items: [
                        {
                            name: 'Characters',
                            href: '#'
                        },
                        {
                            name: 'Comics',
                            href: '#'
                        },
                        {
                            name: 'Movies',
                            href: '#'
                        },
                        {
                            name: 'TV',
                            href: '#'
                        },
                        {
                            name: 'Games',
                            href: '#'
                        },
                        {
                            name: 'Video',
                            href: '#'
                        },
                        {
                            name: 'News',
                            href: '#'
                        },
                    ]
                },
                {
                    title: 'SHOP',
                    items: [
                        {
                            name: 'Shop DC',
                            href: '#'
                        },
                        {
                            name: 'Shop DC Collectibles',
                            href: '#'
                        }, 
                    ]
                },
                {
                    title: 'DC',
                    items: [
                        {
                            name: 'Terms Of Use',
                            href: '#'
                        }, 
                        {
                            name: 'Privacy policy (New)',
                            href: '#'
                        }, 
                        {
                            name: 'Ad Choice',
                            href: '#'
                        }, 
                        {
                            name: 'Advertising',
                            href: '#'
                        }, 
                        {
                            name: 'Jobs',
                            href: '#'
                        }, 
                        {
                            name: 'Subscriptions',
                            href: '#'
                        }, 
                        {
                            name: 'Talent Workshop',
                            href: '#'
                        }, 
                        {
                            name: 'CPSC Certificates',
                            href: '#'
                        }, 
                        {
                            name: 'Ratings',
                            href: '#'
                        }, 
                        {
                            name: 'Shop Help',
                            href: '#'
                        }, 
                        {
                            name: 'Contact Us',
                            href: '#'
                        },  
                    ]
                    
                },
                {
                    title: 'SITES',
                    items: [
                        {
                            name: 'DC',
                            href: '#'
                        },  
                        {
                            name: 'MAD Magazine',
                            href: '#'
                        },  
                        {
                            name: 'DC Kids',
                            href: '#'
                        },  
                        {
                            name: 'DC Universe',
                            href: '#'
                        },  
                        {
                            name: 'DC Power Visa',
                            href: '#'
                        },                    
                    ]
                    
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
        <div class="row col-6 p-0">
            <div class="col-2" v-for="(section, index) in sections" key="index">
                <div class="titles">{{ section.title }}</div>
                <ul>
                    <li v-for="(item, i) in section.items" key="i">
                        <a :href="item.href">
                            {{ item.name }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="col-5 p-0 d-flex justify-content-end position-relative">
            <img src="../../public/img/dc-logo-bg.png" alt="">
        </div>
    </div>

</template>

<style lang="scss" scoped>

.bg-upper-footer{
    background-color: #0282F9;
    position: relative;
}

.titles{
    font-weight: bold;
    font-size: 15px;
    color: white;
}

ul{
    list-style: none;
    padding: 0;
    margin: 0;

    li {
        a{
            font-size: 12px;
            text-decoration: none;
            color: rgba(255, 255, 255, 0.5);
        }
    }
}

img{
    position: absolute;
    top: -150px;
}
</style>
