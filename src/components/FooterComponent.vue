<template>
    <div class="wrapper">
        <div class="container text-black py-5">
            <div class="row">
                <div class="col-4">
                    <div class="address">
                        <h4>
                            Address
                        </h4>
                        <div>382 NE 191st ST # 87394 Miami, FL 33179</div>
                        <div>+1(305)547-9909(9am-5pm EST,Monday -Friday)</div>
                        <div>support@maxcoach.com</div>
                        <div class="social"><a :href="social.link" v-for="(social,index) in socials" :key="index"><i
                                    class="fa-brands " :class="social.iconClass"></i></a>
                        </div>
                    </div>
                </div>
                <div class="col-2" v-for="(item, index) in listLinks" :key="index">
                    <h4>{{ item.title }}</h4>
                    <ul>
                        <li v-for="(link, index) in item.links" :key="index"><a :href="link.link">{{ link.name }}</a>
                        </li>

                    </ul>
                </div>
                <div class="col-4">
                    <div class="instagram">
                        <div>
                            <h4 class=" d-inline-block pe-2">Instagram</h4><span class="fs-5"><a
                                    href="">@maxcoach</a></span>
                        </div>
                        <a href=""><img src="/images/120084500_197897808368764_8114555493043279565_n.jpg" alt=""></a>
                        <a href=""><img src="/images/120012142_177596140500760_8623485824101406058_n.jpg" alt=""
                                class="m-3"></a>
                        <a href=""><img src="/images/120099363_364334431619755_7198812647386067017_n.jpg" alt=""></a>


                    </div>

                </div>
            </div>
        </div>
        <div class="text-center  text-secondary">@ 2020 MACHCOACH ALL RIGHT RESERVED</div>
        <div class="scroll-btn"><a href="#" class=""><i class="fa-solid fa-arrow-up"></i></a></div>
    </div>
</template>

<script>
export default {
    name: 'FooterComponent',
    data() {
        return {
            socials: [
                {
                    name: 'twitter',
                    iconClass: 'fa-twitter',
                    link: ''
                },
                {
                    name: 'facebook',
                    iconClass: 'fa-facebook',
                    link: ''
                },
                {
                    name: 'Instagram',
                    iconClass: 'fa-instagram',
                    link: ''
                },
                {
                    name: 'Linkedin',
                    iconClass: 'fa-linkedin',
                    link: ''
                },
            ],
            listLinks: [
                {
                    title: 'Explore',
                    links: [
                        {
                            name: 'Start here',
                            link: '',
                        },
                        {
                            name: 'Success story',
                            link: '',
                        },
                        {
                            name: 'Blog',
                            link: '',
                        },
                        {
                            name: 'Courses',
                            link: '',
                        },
                        {
                            name: 'Contact us',
                            link: '',
                        },
                    ],
                },
                {
                    title: 'Information',
                    links: [
                        {
                            name: 'Membership',
                            link: '',
                        },
                        {
                            name: 'Purchase guide',
                            link: '',
                        },
                        {
                            name: 'Terms policy',
                            link: '',
                        },
                    ],
                },

            ]
        }
    },

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    padding: 1rem 0;
    position: relative;
}

.address {
    div {
        padding: 0.4rem 0;
        color: $boulder;

        i {
            font-size: 1.2rem;
            padding: 0.5rem;
        }
    }
}

ul {
    list-style: none;
    padding: 0;

    li {
        color: $boulder;
        padding: 0.4rem 0;
    }
}

a {
    text-decoration: none;
    color: $boulder;
    font-weight: 600;

}

a:hover {
    color: $primary-color;
}

.instagram {
    img {
        width: 120px;
    }

    a {
        color: $tulip-tree;
    }
}

.scroll-btn {
    position: absolute;
    bottom: 0;
    right: 0;
    margin: 1rem;

    a {
        text-decoration: none;
        background-color: rgb(222, 102, 28);
        color: $white;
        padding: 1rem 1rem;
        width: 55px;
        display: block;
        text-align: center;

        border-radius: 50%;
    }

}
</style>