<template>
    <div id="landing">
        <div class="layer">
            <nav>
                <div class="logo">
                    <font-awesome-icon icon="paper-plane" />
                    <h3>Travel<span>Kit</span></h3>
                </div>
                <div class="menu">
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Destinations</a></li>
                        <li><a href="#">Gallery</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Hotel</a></li>
                        <li><a href="#">Contact</a></li>
                        <li class="btn"><a href="#">Book Online</a></li>
                    </ul>
                </div>
            </nav>
            <section class="info">
                <h1>Start from $299</h1>
                <h4>Lorem Ipsum</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint obcaecati cumque vitae tempore natus! Harum magni beatae error corporis totam. Voluptatum eveniet delectus vel, cumque optio quam magni nesciunt tempora, corrupti quibusdam doloribus natus quod veritatis obcaecati rerum sit voluptates.</p>
                <button>Start Tour</button>
            </section>
            <section class="booking">
                <div class="booknfo">
                    <h2>Booking<br><span>Information</span></h2>
                </div>
                <form>
                    <label for="Destination">
                        <h4>I Want to:</h4>
                        <input type="text" name="Destination" id="formInput" placeholder="Destination">
                    </label>
                    <label for="Date">
                        <h4>When?</h4>
                        <input type="text" name="Date" id="formInput" placeholder="First day of travel">
                    </label>
                    <label for="Duration">
                        <h4>Until when?</h4>
                        <input type="text" name="Duration" id="formInput" placeholder="Length of travel">
                    </label>
                    <label for="Purpose">
                        <h4>Why?</h4>
                        <input type="text" name="Purpose" id="formInput" placeholder="Purpose">
                    </label>
                </form>
                <button class="bookingSubmit"><font-awesome-icon icon="angle-right" /></button>
            </section>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
/* Navbar styling */ 
    #landing {
        background: url('https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-440379.jpg');
        background-size: cover;
        background-repeat: no-repeat;
    }

    .layer {
        height: 100vh;
        padding: 0 10rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        color: #fff;
        background: rgba(78, 113, 128, 0.1);
    }

    nav {
        display: flex;
        align-items: center;
        justify-content: space-between;
        text-shadow: 0px 0px 4px rgba(0, 0, 0, 0.6);
    }

    ul {
        display: flex;
        align-items: center;
        list-style: none;
    }

    li {
        margin: 0 20px;
        font-weight: bold;
    }

    .btn {
        background: #3374dd;
        font-weight: 600;
        padding: 10px;
        border-radius: 3px;
        text-shadow: none;
        box-shadow: 0px 0px 5px 0px rgba(50, 50, 50, 0.75);
    }

    a {
        color: #fff;
        text-decoration: none;
        transition: .3s ease;
    }

    a:hover {
        color: #ddd;
    }

    .logo {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 1.5rem;
    }

    .logo > * {
        padding: 0 10px;
    }

    .logo h3 {
        font-weight: normal;
    }

    .logo h3 > span {
        font-weight: 600;
    }
/* Landing page info */

    .info {
        text-shadow: 0px 0px 8px rgba(0, 0, 0, 0.8);
        max-width: 50%;
    }

    .info > h1 {
        font-size: 4rem;
    }

    .info > h4 {
        font-size: 2.5rem;
    }

    .info > p {
        margin-top: -2.5rem;
        line-height: 1.5rem;
    }

    .info > button {
        background: none;
        border: 1px solid #fff;
        outline: none;
        color: #fff;
        opacity: 0.7;
        text-shadow: 0px 0px 4px rgba(0, 0, 0, 0.6);
        padding: 10px 15px;
        font-weight: bold;
        font-size: 1.1rem;
        text-transform: uppercase;
        transition: .2s ease;
    }

    .info > button:hover {
        cursor: pointer;
        opacity: 1;
    }

/* Booking */

    .booking {
        display: grid;
        grid-template-columns: 1fr 6fr 0.3fr;
    }

    form {
        display: flex;
        background: #fff;
        justify-content: space-evenly;
        color: #7c7c7c;
    }

    form > label input {
        border: 0.5px solid rgba(122, 122, 122, 0.5);
        padding: 5px;
    }

    .booknfo {
        background: #3374dd;
        padding-left: 2rem;
    }

    .booknfo > h2 {
        font-weight: normal;
        font-size: 1.6rem;
        letter-spacing: 0.5px;
    }

    .booknfo > h2 span {
        font-weight: 600;
        font-size: 1.8rem;
    }

    .booking > button {
        background: #3374dd;
        border: none;
        color: white;
        font-size: 2.5rem;
        outline: none;
        transition: .3s ease;
    }

    .booking > button:hover {
        background: #4689f5;
    }
</style>

