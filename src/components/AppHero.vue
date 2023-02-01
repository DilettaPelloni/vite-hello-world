<script>
    export default {
        data() {
            return {
                img: 'https://unsplash.it/1500/500',
                message: 'Jumbotron'
            }
        }
    }
</script>

<template>
    <div id="jumbo">
        <img :src="img" alt="jumbotron">
        <h2> {{ message }}</h2>
    </div>
</template>

<style scoped>
    #jumbo {
        width: 100%;
        height: 500px;
        position: relative;
        overflow: hidden;
    }

    #jumbo img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    #jumbo h2 {
        margin: 0;
        text-transform: uppercase;
        text-shadow: 0px 0px 10px black ;
        font-size: 4rem;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
</style>