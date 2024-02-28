<script>

import AppHero from './components/AppHero.vue';

export default {
    components: {
        AppHero,
    }
}

</script>


<template>

    <AppHero></AppHero>

    <div class="not-found">

        <h3>
            404
        </h3>
        <h3>
            Not Found
        </h3>

    </div>

</template>


<style>

@import url('https://fonts.googleapis.com/css2?family=VT323&display=swap');

.not-found {
    text-align: center;
    margin-top: 50px;
    font-size: 50px;
}

</style>