<template>
    <main>
        <div class="container">
            <h2>Content goes here </h2>
        </div>
    </main>
</template>

<script>
export default{
    name: 'AppMain'
}

</script>

<style scoped lang="scss">

    @import './src/styles/palette.scss';
    main{
        padding: 65px 0px;
        background-color: $secondary;
        color: #fff;
    }   

</style>