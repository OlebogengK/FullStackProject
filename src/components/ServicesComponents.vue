<template>
    <v-card width="300px" height="450px" id="card" class="pa-4 mt-8">
        <v-img
            height="50px"
            width = "50px"
            :src = "src"
        >
        </v-img>
        <h4 class="mb-6">{{ heading }}</h4>
        <h5>{{ description }}</h5>
    </v-card>
</template>
<script>
export default {
    props: ['heading','description','src'],
}
</script>
<style scoped>
h5{
    font-weight: normal;
    font-size: x-large;
} 
h4{
    font-size: xx-large;
}
</style>