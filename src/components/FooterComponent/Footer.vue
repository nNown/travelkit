<template>
    <div id="footer">
        <div class="logo">
            <font-awesome-icon icon="paper-plane" />
            <h1>Travel<span>Kit</span></h1>
        </div>
        <div class="stuff">
            <p>Footer related stuff</p>
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
    #footer {
        background: #3374dd;
        color: #fff;
        display: flex;
        justify-content: space-between;
        padding: 0 4rem;
    }

    .stuff {
        align-self: center;
        
    }

    .logo {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 1.5rem;
    }

    .logo > * {
        padding: 0 10px;
        font-size: 1.5rem;
    }

    .logo h1 {
        font-weight: normal;
        font-size: 1.5rem;
    }

    .logo h1 > span {
        font-weight: 600;
    }
</style>
