<script>
    export default{
        name: "AppFooter",
        data(){
            return{
                footerLinksSx:[
                    {
                        title:"DC COMICS",
                        links:[
                            'Characters',
                            'Comics',
                            'Movies',
                            'TV',
                            'Games',
                            'Videos',
                            'News'
                        ]
                    },
                    {
                        title:"SHOP",
                        links:[
                            'Shop DC',
                            'Shop DC Collectibles',
                        ]
                    }
                ],
                footerLinksCentro:[
                    {
                        title:"DC",
                        links:[
                            'Terms of Use',
                            'Privacy Policy (new)',
                            'Ad Choices',
                            'Advertising',
                            'Jobs',
                            'Subcriptions',
                            'Talent Workshops',
                            'CPSC Certificates',
                            'Ratings',
                            'Shop Help',
                            'Contact Us'
                        ]
                    }
                ],
                footerLinksDx:[
                {
                        title:"SITES",
                        links:[
                            'DC',
                            'MAD Magazines',
                            'DC Kids',
                            'DC Universe',
                            'DC Power Visa',
                        ]
                    },
                ]
            }
        }
    }
</script>
<template>
    <div id="app-footer">
        <div class="links-container">
            <div>
                <div id="link-sx" v-for="footerLinkSx in footerLinksSx">
            <strong>{{ footerLinkSx.title }}</strong>
            <ul v-for="link in footerLinkSx.links">
                <li>
                    {{ link }}
                </li>
            </ul>
        </div>
            </div>
        <div id="link-centro" v-for="footerLinkCentro in footerLinksCentro">
            <strong>{{ footerLinkCentro.title }}</strong>
            <ul v-for="link in footerLinkCentro.links">
                <li>
                    {{ link }}
                </li>
            </ul></div>
        <div id="link-dx" v-for="footerLinkDx in footerLinksDx">
            <strong>{{ footerLinkDx.title }}</strong>
            <ul v-for="link in footerLinkDx.links">
                <li>
                    {{ link }}
                </li>
            </ul>
        </div>
        </div>
        <img src="../../public/img/dc-logo-bg.png" alt="">
    </div>
</template>
<style scoped>
 #app-footer{
    width: 100%;
    background-image: url('../../public/img/footer-bg.jpg');
    height: 270px;
    position: relative;
    overflow: hidden;
    padding: 30px 200px;
 }

 #app-footer img{
    height: 390px;
    position: absolute;
    right: 230px;
    top: -65px;
 }

 ul{list-style-type: none;
margin: 10px 0;}

 li{
    font-size: 0.54em;
    color: gray;
    line-height: 0.55em;
    cursor: pointer;
 }

 .links-container{
    display: flex;
    gap: 30px;
 }


</style>