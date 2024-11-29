<template>
    <div class="container mt-5">
        <h2 class="mb-4">Educación</h2>
        <ul class="list-group">
            <li class="list-group-item" v-for="(edu,index) in education" :key="index">
                <h5>{{ edu.institute }}</h5>
                <p>{{ edu.degree }} | {{ edu.period }}</p>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Education',
    data() {
        return {
            education: [
                {
                    institute: 'Instituto Universitario de Tecnología READIC (UNIR)',
                    degree: 'TSU en Informática',
                    period: '2008 - 2012'
                },
                {
                    institute: 'Universidad Nacional Experimental “Rafael María Baralt”',
                    degree: 'Licenciado en Educación, mención Matemática y Física',
                    period: '2006 - 2011'
                }
            ],
        };
    }
};
</script>

<style scoped>
.list-group-item {
    margin-bottom: 1rem;
}
</style>