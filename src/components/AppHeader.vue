<script>
    export default{
        data() {
            return {
                
                clothingSection: [
                    {
                        section: 'Donna'
                    },
                    {
                        section:'Uomo'
                    },
                    {
                        section:'Bambini'
                    }
                ],

                logo:'./src/assets/img/boolean-logo.png',

                navSection: [
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    }
                ]
            }
        },
    };
</script>

<template>
    <header>
        <div class="header-container">
            <div class="header-section">
                <div v-for="clothing in clothingSection">
                    {{ clothing.section }}
                </div>
            </div>
    

            <div>
                <img :src="logo" alt="">
            </div>

            <div class="header-section">
                <div v-for="nav in navSection">
                    {{nav.icon}}
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