<script>
export default{
    name:"AppCard",
    data(){
        return{

        }
    },
    props:{
        immagine: String,
        text: String, 
    }
}
</script>
<template>
    <div class="card-container">
                <img :src="immagine" alt="">
                <div class="titolo-card"> {{ text }}</div>
            </div>
</template>
<style lang="scss" scoped>
    .card-container{
        width: calc(100% / 6 - 15px / 6 * 5);

        img{
            width:100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            object-position: top;
        }

        .titolo-card{
            text-transform: uppercase;
            font-size: 0.7em;
        }
    }
</style>