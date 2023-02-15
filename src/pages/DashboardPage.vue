<template>
    <div class="dashboard">
        <NavbarCompenent/>
    </div>
</template>

<script>
import NavbarCompenent from '@/components/NavbarCompenent.vue';

export default {
    name: "DashboardPage",
    components: {
        NavbarCompenent
    }
}
</script>

<style  scoped>
/* @import "../assets/dashboard.css" */
.dashboard{
    /* width: 100vw; */
}
</style>