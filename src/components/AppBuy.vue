<script>
    export default{
        data(){
            return{
                buyObjects:[
                    {
                        title: "digital comics",
                        img:"buy-comics-digital-comics.png"
                    },
                    {
                        title: "DC merchandise",
                        img:"buy-comics-merchandise.png"
                    },
                    {
                        title: "subscriptions",
                        img:"buy-comics-subscriptions.png"
                    },
                    {
                        title: "comic shop locator",
                        img:"buy-comics-shop-locator.png"
                    },
                    {
                        title: "DC power visa",
                        img:"buy-dc-power-visa.svg"
                    }
                ]
            }
        }
    }
</script>
<template>
    <div id="buy">
        <div class="container">
            <a v-for="buyObject in buyObjects">
                <img :src="'../../public/img/' + buyObject.img" alt="">
                {{ buyObject.title }}
            </a>
        </div>
    </div>
</template>

<style scoped lang="scss">
    #buy{
        background-color: #0282F9;
        padding: 35px 0;

        .container{
        margin: 0 200px;
        display: flex;
        align-items: center;
        gap: 40px;
        justify-content: space-evenly;

        a{
        cursor: pointer;
        display: flex;
        align-items: center;
        gap:8px;
        text-transform: uppercase;
        font-size: 0.7em;

        img{
        height: 37px;
        max-width: 45px
    }
    }
    }

    
    }
    
    
    

   


</style>