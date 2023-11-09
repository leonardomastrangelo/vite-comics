<template>
    <section id="up-footer">
        <div class="container">
            <div class="row">
                <!-- left -->
                <div class="col-6 d-flex py-5">
                    <div class="col-3">
                        <h3 class="text-uppercase">dc comics</h3>
                        <ul class="pb-3">
                            <li v-for="(item, index) in dcComics" :key="index">
                                <a @click.prevent class="text-capitalize" :href="item.href">
                                    {{ item.link }}
                                </a>
                            </li>
                        </ul>
                        <h3 class="text-uppercase">shop</h3>
                        <ul>
                            <li v-for="(item, index) in shop" :key="index">
                                <a :href="item.href" @click.prevent>
                                    {{ item.link }}
                                </a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-3">
                        <h3 class="text-uppercase">dc</h3>
                        <ul>
                            <li v-for="(item, index) in dc" :key="index">
                                <a @click.prevent class="text-capitalize" :href="item.href">
                                    {{ item.link }}
                                </a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-3">
                        <h3 class="text-uppercase">sites</h3>
                        <ul>
                            <li v-for="(item, index) in sites" :key="index">
                                <a @click.prevent class="text-capitalize" :href="item.href">
                                    {{ item.link }}
                                </a>
                            </li>
                        </ul>
                    </div>

                </div>
                <!-- right -->
                <div class="col-6 d-flex justify-content-center overflow-hidden">

                    <img src="/images/dc-logo-bg.png" alt="dc-logo">

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "UpFooter",
    data() {
        return {
            dcComics: [
                {
                    link: "characters",
                    href: "#"
                },
                {
                    link: "comics",
                    href: "#"
                },
                {
                    link: "movies",
                    href: "#"
                },
                {
                    link: "tv",
                    href: "#"
                },
                {
                    link: "games",
                    href: "#"
                },
                {
                    link: "news",
                    href: "#"
                }
            ],
            dc: [
                {
                    link: "terms of use",
                    href: "#"
                },
                {
                    link: "privacy policy(New)",
                    href: "#"
                },
                {
                    link: "ad choises",
                    href: "#"
                },
                {
                    link: "advertisements",
                    href: "#"
                },
                {
                    link: "jobs",
                    href: "#"
                },
                {
                    link: "subscriptions",
                    href: "#"
                },
                {
                    link: "talent workshop",
                    href: "#"
                },
                {
                    link: "CPSC certificates",
                    href: "#"
                },
                {
                    link: "CPSC certificates",
                    href: "#"
                },
                {
                    link: "ratings",
                    href: "#"
                },
                {
                    link: "show help",
                    href: "#"
                },
                {
                    link: "contact us",
                    href: "#"
                },
            ],
            sites: [
                {
                    link: "DC",
                    href: "#"
                },
                {
                    link: "MAD magazine",
                    href: "#"
                },
                {
                    link: "DC kids",
                    href: "#"
                },
                {
                    link: "DC universe",
                    href: "#"
                },
                {
                    link: "DC power visa",
                    href: "#"
                },
            ],
            shop: [
                {
                    link: "shop DC",
                    href: "#"
                },
                {
                    link: "DC collectibles",
                    href: "#"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
a {
    color: #7d7171;
    font-size: 0.75em;
}

h3 {
    color: white;
    font-weight: 600;
}

img {
    width: 400px;
    transform: scale(1.4);
}
</style>