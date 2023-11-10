<template>
    <section id="content">
        <!-- jumbotron -->
        <section id="jumbo">
        </section>

        <!-- cards -->
        <div class="container">
            <!-- title -->
            <div class="title">
                current series
            </div>

            <!-- cards content -->
            <div class="row">
                <div class="col-6 col-md-4 col-xl-2" v-for="(card, index) in cards" :key="index">
                    <!-- card component -->
                    <CardDC :media="card.thumb" :title="card.series" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import datas from '../data/dc-comics.json';
import CardDC from './CardDC.vue';
export default {
    name: "MainDC",
    components: {
        CardDC
    },
    data() {
        return {
            cards: datas
        }
    },
    mounted() {
    }

}

</script>

<style lang="scss" scoped>
@use '/src/assets/css/partials/variables.scss' as *;

.title {
    text-transform: uppercase;
    padding: 15px;
    color: white;
    background-color: $dc-primary;
    display: inline-block;
    transform: translateY(-50%);
    font-size: 1.4em;
    font-weight: 600;
}

#jumbo {
    background-image: url('/images/jumbotron.jpg');
    background-size: cover;
    width: 100%;
    height: 45vh;
}
</style>