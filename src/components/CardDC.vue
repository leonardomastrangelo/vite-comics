<template>
    <div>
        <!-- image -->
        <div class="card-container">
            <img class="my-fluid" :src="media" alt="title">
        </div>
        <!-- title -->
        <h5>{{ title.toUpperCase() }}</h5>
    </div>
</template>

<script>
export default {
    name: "CardDC",
    props: {
        media: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>
.my-fluid {
    width: 100%;
    display: block;
}

.card-container {
    width: 100%;
    height: 200px;
    overflow: hidden;
}
</style>