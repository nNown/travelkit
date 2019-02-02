<template>
    <div id="sale">
        <div class="layer">
            <h1>Get 10% off on your next travel</h1>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugit quasi fuga ipsa. <br> Lorem ipsum dolor sit amet.</p>
            <button class="btn">Book now!</button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<style scoped>
    #sale {
        height: 100vh;
        background: url('https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-632852.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
    }

    .layer {
        background: rgba(49, 75, 117, 0.35);
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        text-align: center;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-shadow: 0px 0px 14px rgba(0, 0, 0, .8);
    }

    h1 {
        color: #fff;
        font-size: 4rem;
    }

    p {
        color: #fff;
        margin-top: -1rem;
        font-size: 1.2rem;
    }

    .btn {
        background: #307543;
        padding: 1rem 2rem;
        color: #fff;
        text-shadow: 0px 0px 7px rgba(0, 0, 0, .8);
        text-transform: uppercase;
        border: none;
        border-radius: 8px;
        outline: none;
        transition: .3s ease;
    }

    .btn:hover {
        background: #44a35d;
    }
</style>

