<script>
    export default{

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
                    <div>
                        Informazioni legali
                    </div>

                    <div>
                        Informativa sulla privacy
                    </div>

                    <div>
                        Diritto di recesso
                    </div>
                </div>
            </div>

            <div>
                <div>
                    Trovaci anche su:
                </div>

                <div class="footer-info">
                    <div>
                        emoji
                    </div>

                    <div>
                        emoji
                    </div>

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