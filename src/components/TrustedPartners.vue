<template>
    <div class="my-16 mx-16">
        <div class="d-flex">
            <v-sheet class="elevation-24 mt-4 mr-4" width="50" height="10" id="rect"></v-sheet>
            <h5 class="">You'll be in good company</h5>
        </div>
        <h2 class="my-6">Trusted by leading brands</h2>
        <v-row>
            <v-col v-for="partner in partners">
                <v-img
                    height="250px"
                    width="280px"
                    :src="partner.src"
                >
                </v-img>
            </v-col>
        </v-row>
    </div>
</template>
<script>
import partners from '../assets/partners.json'
export default {
    data() {
         return {
            partners: partners,
        };
    }
}
</script>
<style scoped>
h5{
    font-weight: normal;
    font-size: 30px;
}
#rect{
    background-color: #D100C9;
}
h2{
    font-size: 50px;
}
</style>