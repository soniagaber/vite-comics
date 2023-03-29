<script>
export default{
    data(){
            return{
                navbarLinks:[
                    {
                        label:'CHARACTERS',
                        classe:' '
                    },
                    {
                        label:'COMICS',
                        classe:'cliccata'
                    },
                    {
                        label:'MOVIES',
                        classe:' '
                    },
                    {
                        label:'TV',
                        classe:' '
                    },
                    {
                        label:'GAMES',
                        classe:' '
                    },
                    {
                        label:'COLLECTIBLES',
                        classe:' '
                    },
                    {
                        label:'VIDEOS',
                        classe:' '
                    },
                    {
                        label:'FANS',
                        classe:' '
                    },
                    {
                        label:'NEWS',
                        classe:' '
                    },
                    {
                        label:'SHOP',
                        classe:' '
                    }
                ],
            }
        }
}
</script>
<template>
    <nav>
        <div class="container">
            <img src="../../public/img/dc-logo.png" alt="">
            <div id="nav-links">
                <a id="links-container" v-for="navbarLink in navbarLinks" :class="navbarLink.classe">
                        <strong :class="navbarLink.classe">{{ navbarLink.label }}</strong>
                </a>
            </div>
        </div>
    </nav>
</template>
<style scoped lang="scss">
    nav{
        background-color: white;
        margin-top: 5px;
        height: 80px;
        width: 100%;

    .container{
        margin: 0 200px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        #nav-links{
            display: flex;
            flex-direction: row;
            gap: 22px;
            height: 100%;
            align-items: center;

            a{
                cursor: pointer;
                height: 100%;

                strong:hover{
                    color: #0282F9;
                }
            }
            #links-container{

            font-size: 0.6em;
            color: black;
            height: 100%;
            position: relative;
            display: flex;
            align-items: center;
            }
        }

        img{
        height: 70%;
        }
    }
    }

    .cliccata{
        color: #0282F9;
        ::before{
            content:" ";
            background-color: #0282F9;
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 2.5px;
        }
    }
</style>