<template>
    <aside class="py-5">
        <div class="container d-flex justify-content-between">
            <div>
                <button>sign-up now!</button>
            </div>

            <div class="d-flex">
                <h4 class="text-uppercase pe-3">follow us</h4>
                <ul class="d-flex">
                    <li v-for="(social, index) in socials" class="px-3">
                        <a :href="social.href">
                            <img :src="social.image" :alt="social.image">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </aside>
</template>

<script>
export default {
    name: "DownFooter",
    data() {
        return {
            socials: [
                {
                    image: "/images/footer-facebook.png",
                    href: "#"
                },
                {
                    image: "/images/footer-twitter.png",
                    href: "#"
                },
                {
                    image: "/images/footer-youtube.png",
                    href: "#"
                },
                {
                    image: "/images/footer-pinterest.png",
                    href: "#"
                },
                {
                    image: "/images/footer-periscope.png",
                    href: "#"
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
button {
    text-transform: uppercase;
    padding: 10px;
    border: 2px solid #0282F9;
    background-color: transparent;
    color: white;
}
</style>