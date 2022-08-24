<template>
    <header class="d-flex container">
        <div class="first">
            <img src="../assets/dc-logo.png" alt="DC Logo">
        </div>
        <nav class="second nav-bar">
            <ul class="menu">
                <li v-for="menuItem in menuItems" :key="menuItem" class="menu-item">
                    <a href="">{{ menuItem }}</a>
                </li>
            </ul>
        </nav>      
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            menuItems: [
            'Characters',
            'Comics',
            'Movies',
            'Tv',
            'Games',
            'Collectibles',
            'Videos',
            'Fans',
            'News',
            'Shop'
            ]
        }
    }
}
</script>

<style scoped lang="scss">

    @import './src/styles/palette.scss';
    @import './src/styles/header.scss'

</style>

