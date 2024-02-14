<script>
    export default{

    };
</script>

<template>
    <header>
        <div class="header-container">
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

    @use '../styles/partials/variables' as *;

    header{
        color: white;

        background-color: orange;
        
        .header-container {
            height: $container-height;
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