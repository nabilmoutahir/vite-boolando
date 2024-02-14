<script>
    export default {    
        props: {
                img: String,
                brandName: String,
                itemName: String,
                priceValue: Number
                },
    };
</script>

<template>

    <div class="card">

        <figure>
            <img :src="img" alt="">
        </figure>
        
        <div class="card-text">
            <div class="card-brand">
                {{ brandName }}
            </div>

            <div class="card-name-item">
                {{ itemName }}
            </div>

            <div class="card-price">
                {{ priceValue }}
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

    .card {
        width: calc(100% / 3 - 40px);
        margin: 20px;
        display: flex;
        flex-direction: column;
    }

    img{
        width: 100%;
        object-fit: contain;
    }

    .card-text{
        padding-top: 10px;
    }

    .card-brand {
        font-size: smaller;
    }

    .card-name-item {
        font-weight: bold;
    }

    .card-price {
        font-weight: bolder;
        color: red;
    }

</style>