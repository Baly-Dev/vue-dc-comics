<template>
    <div class="card">
        <div class="card-header">
            <img :src="card.thumb" alt="">
        </div>
        <div class="card-body">
            <h4>{{card.series}}</h4>
        </div>
    </div>
</template>

<script>

export default {
    name: 'ComicCard',
    props: {
        card: Object
    }
}

</script>

<style scoped lang="scss">

    .card{
        margin-bottom: 20px;
        cursor: pointer;

        .card-header{
            padding: 0px 10px;
            margin-bottom: 10px;

            img{
            width: 100%;
            }
        }

        .card-body{
            padding: 0px 10px;

            h4{
                font-size: 0.8em;
                text-transform: uppercase;
                line-height: 1.6em;

            }
        }
    }
</style>