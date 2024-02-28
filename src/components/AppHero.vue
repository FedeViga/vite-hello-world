<script>

import AppTitle from './AppTitle.vue';

export default {

    name: 'AppHero',
    components: {
        AppTitle,
    },

    data() {
        return {

            image: "https://img.freepik.com/free-photo/matrix-hacker-background_23-2150082005.jpg?size=626&ext=jpg&ga=GA1.1.1788068356.1706140800&semt=ais"

        }
    }


}

</script>

<template>

    <div class="container">

        <AppTitle></AppTitle>

        <div class="row">
        
            <div class="col">

                <h2>
                    > Benvenuto nella mia prima App creata con Vite! Purtroppo quest'app non fa ancora niente :(
                </h2>
                
                <div class="buttons">
        
                    <a href="#"> > Link che non porta da nessuna parte</a>
            
                    <div class="button">
                        > Bottone che non fa niente
                    </div>
        
                </div>

            </div>

            <div class="col">

                <img :src="image" alt="immagine">
                
            </div>

        </div>

    </div>

</template>

<style>

.container {
    width: 100%;
    background-color: black;
    color: lime;
    padding: 50px;
}

h2 {
    margin-bottom: 20px;
}

.row {
    display: flex;
    justify-content: center;
    gap: 50px;
}

.buttons {
    margin-left: 20px;
}

a {
    display: inline-block;
    margin-bottom: 20px;
    color: lime;
}

a:hover {
    color: rgb(0, 194, 0);
}

.button {
    width:fit-content;
    border: 2px solid lime;
    border-radius: 20px;
    padding: 6px 10px;
    transition: .2s ease;
}

.button:hover {
    cursor: pointer;
    transform: scale(1.05);
    background-color: lime;
    color: black;
}

img {
    width: 300px;
}

</style>