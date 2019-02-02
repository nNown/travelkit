<template>
    <div id="happy">
        <section class="intro">
            <h1>Our Customers</h1>
            <hr>
        </section>
        <div class="grid">
            <img v-for="img in imgGrid" :src="img">
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            imgGrid: [
                'https://images.pexels.com/photos/450441/pexels-photo-450441.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260',
                'https://images.pexels.com/photos/787452/pexels-photo-787452.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260',
                'https://images.pexels.com/photos/732629/pexels-photo-732629.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260',
                'https://images.pexels.com/photos/618543/pexels-photo-618543.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260',
                'https://images.pexels.com/photos/837129/pexels-photo-837129.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260'
            ]
        }
    }
}
</script>

<style scoped>
    #happy {
        min-height: 50vh;
        margin-top: -1.5rem;
    }

    .grid {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: 1fr 1fr;
        margin: 2rem;
        grid-gap: 2rem;
    }

    .grid > img {
        position: relative;
        width: 100%;
        object-fit: cover;
        align-self: stretch;
        opacity: 0.95;
        transition: .4s ease-in .1s;
    }

    .grid > img:hover {
        opacity: 1;
        transform: scale(1.05);
        z-index: 2;
    }

    .grid > img:nth-of-type(1) {
        grid-column: 1 / 3;
        grid-row: 1 / 3;
    }
</style>


