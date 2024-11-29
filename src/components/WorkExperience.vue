<template>
    <div class="container mt-5">
        <h2 class="mb-4">Experiencia Laboral</h2>
        <div class="row">
            <div class="col-md-6 mb-4" v-for="(job,index) in jobs" :key="index">
                <div class="card">
                    <div class="card-body">
                        <h5 class="card-title">{{ job.company }}</h5>
                        <h6 class="card-subtitle mb-2 text muted">{{ job.period }} - {{ job.position }}</h6>
                        <p class="card-text">{{ job.description }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'WorkExperience',
    data() {
        return {
            jobs: [
                {
                    company: '2Brains',
                    position: 'Desarrollador Front-End',
                    period: 'Julio 2024 - Actualidad',
                    description: 'Renderización de componentes en Angular, integración de APIs, y uso de Google Cloud Platform.'
                },
                {
                    company: 'Acid Labs',
                    position: 'Desarrollador Front-End',
                    period: 'Octubre 2022 - Mayo 2024',
                    description: 'Desarrollo de aplicaciones web DaaS con Micro Frontend, incluyendo proyectos clave como Daas-BFF.'
                },
            ],
        };
    }
};
</script>

<style scoped>
.card{
    border: none;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
</style>