<template>
    <header class="container d-flex justify-content-between">
        <!-- LOGO -->
        <div class="py-4">
            <img src="/images/dc-logo.png" alt="dc-logo">
        </div>
        <!-- NAV-BAR -->
        <ul class="d-flex align-items-stretch">
            <li v-for="(item, index) in headerLinks" :key="index" class="px-3 d-flex align-items-center position-relative">
                <a :class="{ 'active-item': item.focused }" @click.prevent="activeLink(item)" :href="item.href">{{
                    item.link.toUpperCase()
                }}</a>
                <div class="active-bar" v-show="item.focused">
                </div>
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
                    focused: true,
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
    },
    methods: {
        activeLink(link) {
            this.headerLinks.forEach((link => {
                link.focused = false
            }))
            link.focused = !link.focused
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

    .active-bar {
        width: 100%;
        height: 5px;
        background-color: #0282F9;
        position: absolute;
        bottom: 0;
        left: 0;
    }

}

.active-item {
    color: #0282F9;
}
</style>