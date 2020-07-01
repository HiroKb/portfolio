<template>
    <v-container>
        <div class="bloc-logo">
            <canvas id="logo-canvas"></canvas>
            <h1 class="logo-mask">Hiro'sPortfolio</h1>
        </div>
    </v-container>
</template>

<script>
    import Granim from 'granim'
    export default {
        name: 'Top',
        data () {
            return {
                granim: {}
            }
        },
        mounted() {
            this.granim = new Granim({
                element: '#logo-canvas',
                direction: 'left-right',
                states : {
                    "default-state": {
                        gradients: [
                            ['#EB3349', '#F45C43'],
                            ['#FF8008', '#FFC837'],
                            ['#4CB8C4', '#3CD3AD'],
                            ['#24C6DC', '#514A9D'],
                            ['#FF512F', '#DD2476'],
                            ['#DA22FF', '#9733EE']
                        ],
                        transitionSpeed: 2000
                    }
                }
            })
            scrollTo(0, 0)
        }
    }
</script>

<style scoped>
    .container{
        height: 100%;
        display: flex;
        align-items: center;
    }
    .bloc-logo {
        position: relative;
        width: 382px;
        height: 198px;
        float: left;
    }

    .bloc-logo canvas,
    .bloc-logo .logo-mask {
        display: block;
        width: 382px;
        height: 198px;
    }

    .bloc-logo .logo-mask {
        position: absolute;
        top: -1px;
        left: 0;
        background-size: 400px;
        background-image: url("../assets/topimage.png");
        text-indent: -9999px;
    }

    @media screen and (max-width: 599px){
        .container{
            height: 80%;
        }
        .bloc-logo{
            width: 300px;
            height: 160px;
        }
        .bloc-logo canvas,
        .bloc-logo .logo-mask {
            width: 300px;
            height: 160px;
        }
        .bloc-logo .logo-mask{
            background-size: 312px;
        }
    }
</style>

