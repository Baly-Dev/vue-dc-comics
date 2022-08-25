<template>
    <main>
        <div class="first">
        </div>
        <div class="second">
            <div class="container relative-wrapper">
                <h2>Current Series</h2>
                    <ComicCardsGrid />
                <button class="btn">Load More</button>
            </div>
        </div>
    </main>
</template>

<script>
import ComicCardsGrid from './ComicCardsGrid.vue';

export default{
    name: "AppMain",
    components: { ComicCardsGrid }
}
</script>

<style scoped lang="scss">
    @import './src/styles/palette.scss';
    
    main{
        .first{
            padding: 200px 0px;
            background-image: url(../assets/img/jumbotron.jpg);
            background-position:top;
            background-size: cover;
            background-repeat: no-repeat;
        }

        .second{
            padding: 65px 0px;
            background-color: $secondary;
            color: #fff;

            .relative-wrapper{
                position: relative;
                display: flex;
                flex-direction: column;
                
                
                h2{
                    position: absolute;
                    top: -85px;
                    background-color: $primary;
                    padding: 12px 15px;
                    text-transform: uppercase;
                    font-size: 1.2em;
                }

                .btn{
                    border: 2px solid $primary;
                    padding: 12px 15px;
                    background-color: $primary;
                    color: #fff;
                    text-transform: uppercase;
                    cursor: pointer;
                    width: 12%;
                    margin: 0 auto;
                }
            }
        }
    }   
</style>