<template>
  <header class="container">
        <div class="logo">
            <img src="../assets/dc-logo.png" />
        </div>
        <div class="menu">
            <ul>
                <li 
                v-for="(item, i) in navbarItems" 
                :key="i">
                    <a :href="item.href">{{ item.title }}</a>
                </li>
            </ul>
        </div>
  </header>
</template>

<script>
export default {
    name: "Header",
    data(){
        return {
            navbarItems: [
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
                    title: "Collectibles",
                    href: "#",
                },
                {
                    title: "Videos",
                    href: "#",
                },
                {
                    title: "Fans",
                    href: "#",
                },
                {
                    title: "News",
                    href: "#",
                },
                {
                    title: "Shop",
                    href: "#",
                },
            ]
        }
    }
}
</script>

<style>

</style>