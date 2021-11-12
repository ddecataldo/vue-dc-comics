<template>
    <footer>
        <div class="bg-primary">
            <div class="container">
                <div class="row">
                    <div v-for="(imageService, i) in listImageService" :key="i" class="column5">
                        <img :src="require('../assets/'+ imageService.path )">
                        <span>{{ imageService.text }}</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="bkg">
            <div class="container">
                <div class="row">
                    <div class="menu_footer">
                        <div class="menu_1">
                            <div class="menu_1_1">
                                <h3>DC COMICS</h3>
                                <ul>
                                    <li v-for="(items_1, i) in listItemsFooter_1" :key="i">
                                        <a :href="items_1.href">{{ items_1.title }}</a>
                                    </li>
                                </ul>    
                            </div>
                            <div class="menu_1_2">
                                <h3>SHOP</h3>
                                <ul>
                                    <li v-for="(items_2, i) in listItemsFooter_2" :key="i">
                                        <a href="items_2.href">{{ items_2.title }}</a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                        <div class="menu_2">
                            <h3>DC</h3>
                            <ul>
                                <li v-for="(items_3, i) in listItemsFooter_3" :key="i">
                                    <a href="items_3.href">{{ items_3.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="menu_3">
                            <h3>SITES</h3>
                            <ul>
                                <li v-for="(items_4, i) in listItemsFooter_4" :key="i">
                                    <a href="items_4.href">{{ items_4.title }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="claimer">
                            <p>All Site Content TM and © 2020 DC Entertainment, unless otherwise <a href="#">noted here</a>. All rights reserved.<br> 
                            <a href="#"> Cookies Settings</a></p>
                        </div>    
                    </div>
                </div>
            </div>
        </div> 
        <div class="bg-dark">
            <div class="container">
                <div class="row">
                    <div class="column1">
                        <a href="#" class="btn btn-primary">sign-up now!</a>
                    </div>
                    <div class="column2">
                        <span>Follow Us</span>
                        <img v-for="(imageSocial, i) in listImageSocial" :key="i" :src="require('../assets/'+ imageSocial.path )" :alt="imageSocial.alt">
                    </div>
                </div>
            </div>
        </div>   
    </footer>
</template>

<script>
export default {
    data(){
        return {
            listItemsFooter_1: [
                {
                    title: "Characters",
                    href: "#",
                },
                {
                    title: "Comics",
                    href: "#",
                },
                {
                    title: "Movies",
                    href: "#",
                },
                {
                    title: "TV",
                    href: "#",
                },
                {
                    title: "Games",
                    href: "#",
                },
                {
                    title: "Videos",
                    href: "#",
                },
                {
                    title: "News",
                    href: "#",
                }
            ],
            listItemsFooter_2: [
                {
                    title: "Shop DC",
                    href: "#",
                },
                {
                    title: "Shop DC Collectibles",
                    href: "#",
                },
            ],
            listItemsFooter_3: [
                {
                    title: "Terms of Use",
                    href: "#",
                },
                {
                    title: "Privacy Policy (New)",
                    href: "#",
                },
                {
                    title: "Ad Choices",
                    href: "#",
                },
                {
                    title: "Advertising",
                    href: "#",
                },
                {
                    title: "Jobs",
                    href: "#",
                },
                {
                    title: "Subscriptions",
                    href: "#",
                },
                {
                    title: "CPSC Certificates",
                    href: "#",
                },
                {
                    title: "Ratings",
                    href: "#",
                },
                {
                    title: "Shop Help",
                    href: "#",
                },
                {
                    title: "Contact Us",
                    href: "#",
                },
            ],
            listItemsFooter_4: [
                {
                    title: "DC",
                    href: "#",
                },
                {
                    title: "MAD Magazine",
                    href: "#",
                },
                {
                    title: "DC Kids",
                    href: "#",
                },
                {
                    title: "DC Universe",
                    href: "#",
                },
                {
                    title: "DC Power Visa",
                    href: "#",
                },
            ],
            listImageSocial: [
                {
                 path: "footer-facebook.png",
                 alt: "Seguici su Facebook"
                },
                {
                 path: "footer-twitter.png",
                 alt: "Seguici su Twitter"
                },
                {
                 path: "footer-youtube.png",
                 alt: "Seguici su YouTube"
                },
                {
                 path: "footer-pinterest.png",
                 alt: "Seguici su Pintarest"
                },
                {
                 path: "footer-periscope.png",
                 alt: "Seguici su Periscope"
                }
                
            ],
            listImageService: [
                {
                    path: "buy-comics-digital-comics.png",
                    text: "digital comics",
                },
                {
                    path: "buy-comics-merchandise.png",
                    text: "dc merchandise",
                },
                {
                    path: "buy-comics-subscriptions.png",
                    text: "subscription",
                },
                {
                    path: "buy-comics-shop-locator.png",
                    text: "comic shop locator",
                },
                {
                    path: "buy-dc-power-visa.svg",
                    text: "dc power visa",
                },
            ]

        }
    }
        
}
</script>

<style>

</style>

