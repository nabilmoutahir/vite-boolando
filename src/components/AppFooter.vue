<script>
    export default{
        data() {
            return {
                
                footerInfos:[
                    {
                        info:'Informazioni legali'
                    },
                    {
                        info:'Informativa sulla privacy'
                    },
                    {
                        info:'Diritto di recesso'
                    }
                ],

                footerLinks:[
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    },
                    {
                        icon:'emoji'
                    },
                ]

            }
        },
    };
</script>

<template>
    <footer>
        <div class="footer-container">
            <div>
                <div>
                    Boolando s.r.l
                </div>

                <div class="footer-info">
                    <div v-for="footerInfo in footerInfos">
                        {{footerInfo.info}}
                    </div>
                </div>
            </div>

            <div>
                <div>
                    Trovaci anche su:
                </div>

                <div class="footer-info">
                    <div v-for="footerLink in footerLinks">
                        {{footerLink.icon}}
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>

    @use '../styles/partials/variables' as *;

    footer {
       
        position: sticky;

        background-color: black;

        color: white;

        .footer-container {
            height: $container-height;
            width: 80vw;
            padding: 30px 20px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .footer-info {
            padding-top: 10px;
            display: flex;
            justify-content: space-between;
        }

        .footer-info > div{
            font-size: smaller;
            padding-right: 10px;
        }
    }


</style>