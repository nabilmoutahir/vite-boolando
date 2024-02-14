<script>
    export default{

    };
</script>

<template>
    <header>
        <div class="content-container">
            <div class="header-section">
                <div>
                    Donna
                </div>

                <div>
                    Uomo
                </div>

                <div>
                    Bambini
                </div>
            </div>
    

            <div>
                <img src="../assets/img/boolean-logo.png" alt="">
            </div>

            <div class="header-section">
                <div>
                    emoji
                </div>

                <div>
                    emoji
                </div>

                <div>
                    emoji
                </div>
            </div>
        </div>
    </header>
    
</template>

<style lang="scss" scoped>

    header{
        font-size: small;

        color: white;

        background-color: orange;
        
        .content-container {
            width: 80vw;
            margin: auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .header-section{
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .header-section > div {
            padding: 20px;
        }

        img {
            width: 100px;
        }
    }

</style>