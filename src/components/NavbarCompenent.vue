<template>
    <section class="navigation">
        <div class="logo">
            <img src="../assets/images/logo.png" alt="">
            <h2>P Force</h2>

        </div>
        <div class="n1">
            <div class="search">
                <i class="far fa-search"></i>
                <input type="search" placeholder="Search">
            </div>
        </div>

        <div class="profile">
            <i class=" far fa-bell"></i>
            <img src="../assets/images/1.jpg" alt="">
        </div>
    </section>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .navigation{
        display: flex;
        width: 100%;
        justify-content: space-around;
        align-items: center;
    }
    .navigation img{
        width: 3rem;
    }
    .logo{
        display: flex;
        gap: 2rem;
    }
</style>