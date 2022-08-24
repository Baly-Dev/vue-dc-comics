<template>
    <footer>
        <!-- Footer First -->
        <div class="first">
            <div class="container">
                <ul class="categories">
                    <li v-for="category in categoriesList" :key="category">
                        <img :src="category.img" :alt="category.name">
                        <p>{{category.name}}</p>
                    </li>
                </ul>
            </div>
        </div>

        <!-- Footer Second -->
        <div class="second">
            <div class="container">
                <div class="wrapper">
                    <div class="left">
                        <nav v-for="(menu, i) in menuItems" :key="menu">
                            <h4 class="title">{{ menu.title }}</h4>
                            <ul class="menu">
                                <li class="menu-item" v-for="item in menuItems[i].items" :key="item">
                                    <a href="#">
                                        {{item}}
                                    </a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <div class="right">

                    </div>
                </div>
            </div>
        </div>
        
        <!-- Footer Third -->
        <div class="third">
            <div class="container wrapper">
                <div class="btn-wrapper">
                    <button class="btn">Sign-up Now!</button>
                </div>
                <div class="social-wrapper">
                    <p>Follow Us</p>
                    <ul class="social">
                        <li v-for="socialItem in socialItems" :key="socialItem" class="social-item">
                            <a href="#"><img :src="socialItem" alt=""></a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

export default {
    name: 'AppFooter',
    data(){
        return{
            categoriesList: [
                {
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics'
                },
                {
                    img: require('../assets/img/buy-comics-merchandise.png'),
                    name: 'DC Merchandise'
                },
                {
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                    name: 'Subscription'
                },
                {
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                    name: 'Comic Shop Locator'
                },
                {
                    img: require('../assets/img/buy-dc-power-visa.png'),
                    name: 'DC Power Visa'
                }
            ],
            menuItems: [
                {
                    title: 'Dc Comics',
                    items: [
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum'
                    ]
                },
                {
                    title: 'Dc',
                    items: [
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum'
                    ]
                },
                {
                    title: 'Sites',
                    items: [
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum'
                    ]
                },
                {
                    title: 'Shop',
                    items: [
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum',
                        'Lorem ipsum'
                    ]
                }
            ],
            socialItems: [
                require('../assets/img/footer-facebook.png'),
                require('../assets/img/footer-periscope.png'),
                require('../assets/img/footer-pinterest.png'),
                require('../assets/img/footer-twitter.png'),
                require('../assets/img/footer-youtube.png')
            ]
        }
    }
}

</script>

<style scoped lang="scss">

@import '../styles/palette.scss';
@import '../styles/footer.scss'

</style>