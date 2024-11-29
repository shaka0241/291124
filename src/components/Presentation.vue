<template>
    <div class="container text-center mt-5">
        <h1>{{ name }}</h1>
        <p class="lead">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: 'Presentation',
    data() {
        return {
            name: 'Alberto Rojas - Desarrollador Front-End',
            description: 'Desarrollador Front-End con experiencia en Javascript, VueJS y ReactJS'
        };
    }
};
</script>

<style scoped>
.container {
    padding: 2rem;
}
</style>