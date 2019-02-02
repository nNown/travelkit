<template>
    <div id="destinations">
        <section class="intro">
            <h1>Popular Packages</h1>
            <hr>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam obcaecati dolor, alias animi laudantium sequi? Iste minima quis inventore eveniet. <br>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </section>
        <section class="grid">
            <div v-for="{title, img} in gridObject" :style="{background: `url(${img})`, backgroundSize: 'cover'}">
                <div class="layer">
                    <h1>{{ title }}</h1>
                    <button>Book now!</button>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            gridObject: {
                first: {title: 'Above Greece', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-183262.jpg'},
                second: {title: 'Hawaiian Cruise', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-68962.jpg'},
                third: {title: 'Beneath Australia', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-211853.jpg'},
                fourth: {title: 'On the Top of the World', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-11505.jpg'},
                fifth: {title: 'Snow Chill', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-336471.jpg'},
                sixth: {title: 'Feel the Sakura Blossom', img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-211553.jpg'}
            }
        }
    }
}
</script>

<style scoped>
    .grid {
        display: flex;
        flex-wrap: wrap;
        padding: 1rem 9rem;
    }
    
    .grid > div {
        flex-basis: 30%;
        flex-grow: 1;
        min-height: 300px;
        margin: 1rem;
        border-radius: 10px;
    }

    div {
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        color: #fff;
        text-shadow: 0px 0px 4px rgba(0, 0, 0, 0.6);
    }

    .layer {
        position: relative;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(9, 47, 71, 0.35);
        transition: .3s ease;
        border-radius: 10px;
    }

    .layer:hover {
        background: none;
    }

    .grid > div > .layer > * {
        margin: 2rem 0 2.5rem 0;
        padding: 0 2.5rem;
    }

    .grid > div > .layer > h1 {
        margin: 0;
        font-size: 2rem;
    }

    .grid > div > .layer > button {
        position: relative;
        max-width: 150px;
        margin-left: 2.5rem;
        font-size: 1.2rem;
        padding: 10px;
        border-radius: 8px;
        background: #3374dd;
        text-shadow: 0px 0px 4px rgba(0, 0, 0, 0.6);
        border: none;
        outline: none;
        color: white;
        transition: .3s ease;
    }

    .grid > div > .layer > button:hover {
        cursor: pointer;
        background: #4689f5;
    }

</style>


