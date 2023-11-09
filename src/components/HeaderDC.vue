<template>
    <header class="container d-flex justify-content-between">
        <!-- LOGO -->
        <div class="py-4">
            <img src="/images/dc-logo.png" alt="dc-logo">
        </div>
        <!-- NAV-BAR -->
        <ul class="d-flex align-items-center">
            <li v-for="(item, index) in headerLinks" :key="index" class="px-3">
                <a @click.prevent :href="item.href">{{ item.link.toUpperCase() }}</a>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: "HeaderDC",
    data() {
        return {
            headerLinks: [
                {
                    link: "characters",
                    focused: false,
                    href: "#"
                },
                {
                    link: "comics",
                    focused: false,
                    href: "#"
                },
                {
                    link: "movies",
                    focused: false,
                    href: "#"
                },
                {
                    link: "tv",
                    focused: false,
                    href: "#"
                },
                {
                    link: "games",
                    focused: false,
                    href: "#"
                },
                {
                    link: "collectibles",
                    focused: false,
                    href: "#"
                },
                {
                    link: "videos",
                    focused: false,
                    href: "#"
                },
                {
                    link: "fans",
                    focused: false,
                    href: "#"
                },
                {
                    link: "news",
                    focused: false,
                    href: "#"
                },
                {
                    link: "shop",
                    focused: false,
                    href: "#"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
ul {
    list-style: none;

    a {
        text-decoration: none;
        font-weight: 600;
    }
}
</style>