<template>
    <div id="grid">
        <section class="intro">
            <h1>Top Destinations</h1>
            <hr>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos saepe, autem nostrum alias in dicta. <br> Lorem ipsum dolor sit amet consectetur adipisicing.</p>
        </section>
        <section class="destinations">
            <div v-for="{title, desc, img} in destinations">
                <img :src="img">
                <h1>{{ title }}</h1>
                <p>{{ desc }}</p>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            destinations: {
                Australia: {
                    title: 'Sydney',
                    desc: 'Opera House',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-95860.jpg'
                },
                France: {
                    title: 'France',
                    desc: 'Eiffel Tower',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-136666.jpg'
                },
                India: {
                    title: 'India',
                    desc: 'Taj Mahal',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-21888.jpg'
                },
                Russia: {
                    title: 'Russia',
                    desc: 'Moscow',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-24856.jpg'
                },
                America: {
                    title: 'USA',
                    desc: 'Statue of Liberty',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-434424.jpg'
                },
                England: {
                    title: 'Great Britain',
                    desc: 'London Eye',
                    img: 'https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-303015.jpg'
                }
            }
        }
    }
}
</script>

<style scoped>
    #grid {
        height: 50vh;
    }

    .destinations {
        display: flex;
        justify-content: space-evenly;
        padding: 0 10rem;
    }

    .destinations > div {
        flex-basis: 15%;
        margin-top: 2rem;
    }

    .destinations > div > h1 {
        font-size: 1.2rem;
        margin-top: -0.05rem;
    }

    .destinations > div > p {
        margin-top: -.6rem;
        font-size: 1rem;
    }

    .destinations > div > img{
        position: relative;
        width: 100%;
        height: 50%;
        object-fit: cover;
        border-radius: 4px;
        opacity: 0.9;
        transition: .2s ease;
    }

    .destinations > div > img:hover {
        opacity: 1;
    }

    .intro {
        margin-top: 2rem;
    }
</style>

