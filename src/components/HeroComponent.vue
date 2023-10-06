<template>
     <v-img
        height="100vh"
        width="100vw"
        src="/confidence.jpeg"
        class="my-0 py-0"
        cover
    >
        <div
            class="d-flex h-100 align-start flex-column justify-end ml-16" id="hero" width="200"
        >
            <div><h1 class="mb-4">Live with Confidence</h1></div>
            <div><h4 class="mb-10">Jose Mourinho brings confidence to pan-African Sanlam <br/>campaign.</h4></div>
            <div class="mb-16" id="heroText"><v-btn rounded="xl" id="heroButton" color="#70259B">Lets Talk</v-btn></div>
        </div>
    </v-img>
</template>
<script>
export default {
    
}
</script>
<style scoped>
#hero h1{
    color: white;
    font-size: 50px;
}
#hero h4{
    color: white;
    font-size: x-large;
}
#heroButton{
    margin-bottom: 120px;
}
#hero{
    overflow-y: auto;
    width: fit-content;
    block-size: fit-content;
}
</style>