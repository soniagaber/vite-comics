<script>
export default{
    name:"AppFollow",
    data(){
        return{
            iconsObject:[
                'footer-facebook.png',
                'footer-twitter.png',
                'footer-youtube.png',
                'footer-pinterest.png',
                'footer-periscope.png'
            ]

        }
    }
}
</script>
<template>
    <div id="foll">
        <button> <strong>SIGN-UP NOW!</strong> </button>
        <div id="flex-right">
            <div id="follow"><strong>FOLLOW US</strong>
                </div>
            <div id="icons-container">
                <a id="foll-icons" v-for="iconObject in iconsObject">
                <img :src="'../../public/img/' + iconObject">
            </a>
            </div>
        </div>
    </div>
</template>
<style scoped lang="scss">

#foll{
 background-color:#303030;
 height: 70px;
 width: 100vw;
 padding: 0 200px;
 display: flex;
 justify-content: space-between;
 align-items: center;
 button{
    height: 40px;
    font-size: 0.7em;
    padding: 0px 7px;
    color: white;
    background-color: transparent;
    border-color: #0282F9;
    cursor: pointer;
 }

 #follow{
    color: #0282F9;
    cursor: pointer;
 }

 #flex-right{
    display: flex;
    flex-direction: row;
    gap: 15px;

    #icons-container{
        display: flex;
        gap: 15px;

        img{
            height: 25px;
            cursor: pointer;
        }
    }
 }
}
    
</style>