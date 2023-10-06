<template>
    <div class="mx-16 mt-16">
        <div class="d-flex">
            <v-sheet class="elevation-24 mt-4 mr-4" width="50" height="10" id="rect"></v-sheet>
            <h5 class="">What we do</h5>
        </div>
        <h2>We offer a complete range of bespoke design and development services to help turn your ideas into digital masterpieces</h2>
        <div class="d-md-flex justify-space-between">
            <div class="" v-for="service in services">
                <Service :src="service.src" :description="service.description" :heading="service.heading"/>
            </div>
        </div>
    </div>
</template>
<script>
import services from '../assets/services.json'
import Service from '@/components/ServicesComponents.vue'
export default {
    data() {
         return {
            services: services,
        };
    },
    components: {
        Service
    }
}
</script>
<style scoped>
h5{
    font-weight: normal;
    font-size: 30px;
}
h2{
    font-size: 50px;
}
span{
    color: #D100C9;
}
#rect{
    background-color: #D100C9;
}
</style>