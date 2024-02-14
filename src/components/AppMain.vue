<script>

    import AppCard from './AppCard.vue';

    
    export default{
        data() {
            return {
                
                cards: [
                    {
                    id: 1,
                    frontImage: '1.webp',
                    backImage: '1b.webp',
                    brand: "Levi's",
                    name: 'Relaxed Fit',
                    price: 29.99,
                    isInFavorites: true,
                    badges: [
                        {
                        type: 'tag',
                        value: 'Sostenibilità',
                        },
                        {
                        type: 'discount',
                        value: '-50%',
                        },
                    ],
                    },
                    {
                    id: 2,
                    frontImage: '2.webp',
                    backImage: '2b.webp',
                    brand: 'Guess',
                    name: 'Roses Tee',
                    price: 20.99,
                    isInFavorites: true,
                    badges: [
                        {
                        type: 'discount',
                        value: '-30%',
                        },
                    ],
                    },
                    {
                    id: 3,
                    frontImage: '3.webp',
                    backImage: '3b.webp',
                    brand: 'Come Zucchero Filato',
                    name: 'Voglia di colori pastello',
                    price: 129.99,
                    isInFavorites: false,
                    badges: [
                        {
                        type: 'discount',
                        value: '-30%',
                        },
                    ],
                    },
                    {
                    id: 4,
                    frontImage: '4.webp',
                    backImage: '4b.webp',
                    brand: "Levi's",
                    name: 'Tee Unisex',
                    price: 14.99,
                    isInFavorites: false,
                    badges: [
                        {
                        type: 'tag',
                        value: 'Sostenibilità',
                        },
                        {
                        type: 'discount',
                        value: '-50%',
                        },
                    ],
                    },
                    {
                    id: 5,
                    frontImage: '5.webp',
                    backImage: '5b.webp',
                    brand: 'Maya Deluxe',
                    name: 'Stripe Bodice',
                    price: 99.99,
                    isInFavorites: true,
                    badges: [
                        {
                        type: 'tag',
                        value: 'Sostenibilità',
                        },
                        {
                        type: 'discount',
                        value: '-50%',
                        },
                    ],
                    },
                    {
                    id: 6,
                    frontImage: '6.webp',
                    backImage: '6b.webp',
                    brand: 'Esprit',
                    name: 'Maglione - Black',
                    price: 29.99,
                    isInFavorites: true,
                    badges: [
                        {
                        type: 'tag',
                        value: 'Sostenibilità',
                        },
                    ],
                    },
                ],

            }
        }, 
        
        components: { AppCard },

    };
</script>

<template>
    <main>
        <div class="main-container">
            
            <AppCard 
            v-for="card in cards" 
            :img="'../src/assets/img/' + card.frontImage"
            :brandName="card.brand"
            :itemName="card.name"
            :priceValue="card.price"
            ></AppCard>

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