<script>

import AppCard from './AppCard.vue';

import axios from 'axios';


export default {
    data() {
        return {

            cards: [],

        }
    },

    components: { AppCard },

    created() {
        axios.get('http://localhost:3000/products').then((res) => {
            console.log(res.data)
            this.cards = res.data
        })
    },

};
</script>

<template>
    <main>
        <div class="main-container">

            <AppCard v-for="card in cards" :img="'../src/assets/img/' + card.frontImage" :brandName="card.brand"
                :itemName="card.name" :priceValue="card.price"></AppCard>

        </div>
    </main>
</template>

<style scoped>
.main-container {
    height: calc(100vh - 110px);
    width: 80vw;
    margin: auto;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    overflow-y: scroll;
    overflow-x: hidden;
}
</style>