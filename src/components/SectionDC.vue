<template>
    <section id="buy-links">
        <div class="container py-5">
            <div class="row justify-content-around align-items-center">
                <div class="col-12 col-lg-2" v-for="(item, index) in buyList" :key="index">
                    <div class="d-flex align-items-center justify-content-center py-2">
                        <img class="comic-item" :src="item.img" :alt="item.text">
                        <a :href="item.href">
                            {{ item.text.toUpperCase() }}
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "SectionDC",
    data() {
        return {
            buyList: [
                {
                    img: "/images/buy-comics-digital-comics.png",
                    text: "digital comics",
                    href: "#"
                },
                {
                    img: "/images/buy-comics-merchandise.png",
                    text: "dc merchandise",
                    href: "#"
                },
                {
                    img: "/images/buy-comics-subscriptions.png",
                    text: "subscription",
                    href: "#"
                },
                {
                    img: "/images/buy-comics-shop-locator.png",
                    text: "comic shop locator",
                    href: "#"
                },
                {
                    img: "/images/buy-dc-power-visa.svg",
                    text: "dc power visa",
                    href: "#"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.comic-item {
    width: 60px;
    padding-right: 20px;
    display: block;
}

a {
    color: white;
    display: block;
}
</style>