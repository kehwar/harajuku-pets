<template>
    <div class="container">
        <HarajukuLogo class="logo"></HarajukuLogo>
        <p>¡Vive Miau!</p>
        <p>¡Siente Guau!</p>
    </div>
</template>

<script>
import HarajukuLogo from '~/components/harajukuLogo.vue'
export default {
    name: 'IndexPage',
    components: { HarajukuLogo },
}
</script>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
}

.logo {
    height: 100px;
}

p {
    text-align: center;
}
</style>
