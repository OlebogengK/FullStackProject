<template>
    <div class="mt-16" id="contact">
        <div class="d-flex mx-16 mb-16">
            <v-sheet class="elevation-24 mt-12 mr-4" width="50" height="10" id="rect"></v-sheet>
            <h5 class="mt-8">Contact Us</h5>
        </div>
        <v-row class="mx-16">
            <v-col cols="8">
                <h2>Have a project in mind?</h2>
                <h2>Let's make it happen</h2>
            </v-col>
            <v-col>
                <div id="address">
                    <h5>22 Street Name, Suburb, 8000, Cape Town, South Africa +27214310001 enquire@website.co.za</h5>
                </div>
            </v-col>
        </v-row>
        <v-row class="mt-16 mx-16 pb-10">
            <v-col>
                <h5>Terms of service</h5>
                <h5>Privacy policy</h5>
                <h5>Impressum</h5>
            </v-col>
            <v-col>
                <h5>Facebook</h5>
                <h5>Instagram</h5>
                <h5>Twitter</h5>
            </v-col>
            <v-col>
                <h5>Github</h5>
                <h5>Linkedin</h5>
                <h5>Teams</h5>
            </v-col>
            <v-col>
                <h5>Youtube</h5>
                <h5>Behance</h5>
                <h5>Dribble</h5>
            </v-col>
            <v-col>
                <h5>Explore open jobs</h5>
                <h5></h5>
                <h5>©2000-2023 Company Name</h5>
            </v-col>
        </v-row>
    </div>
</template>
<script>
export default {
    
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
#contact{
    background-color: #70259B;
    color: white;
}
h2{
    font-size: 40px;
}
#address{
    width: 490px;
}
</style>