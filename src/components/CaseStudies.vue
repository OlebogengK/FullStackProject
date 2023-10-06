<template>
    <div class="mx-16 mt-16">
        <div class="d-flex">
            <v-sheet class="elevation-24 mt-4 mr-4" width="50" height="10" id="rect"></v-sheet>
            <h5 class="">Case Studies</h5>
        </div>
        <v-carousel cycle height="400" hide-delimiter-background show-arrows="hover" class="my-10">
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
                :src="item.src"
                id="image"
            >
                <div class="d-flex d-md-none justify-center">
                    <h3>{{ item.heading }}</h3>
                </div>
                <div class="d-flex justify-end fill-height align-center flex-column w-75 ml-10" id="caseStudies">
                    <div class="w-25 d-none d-md-flex">
                        <v-sheet class="elevation-24 mt-4 mr-4" width="50" height="10" id="rect"></v-sheet>
                    </div>
                    <div class="w-25 d-none d-md-flex">
                        <h3>{{ item.heading }}</h3>
                    </div>
                    <div class="w-25 d-none d-md-flex">
                        <h4 class="mb-5">{{ item.description }}</h4>
                    </div>
                </div>
            </v-carousel-item>
        </v-carousel>
    </div>
</template>
<script>
export default {
    data () {
      return {
        items: [
          {
            src: '/dragon.jpeg',
            heading: 'The Savings Jar',
            description: 'Grow your savings treasure and grow your dragon',
          },
          {
            src: '/olympian.jpeg',
            heading: 'The Olympian',
            description: 'The only athlete in the world to do her Olympic routine in 2020',
          },
          {
            src: '/skhokho.jpeg',
            heading: 'Skhokho seMali',
            description: 'Helping South Africans become #CashCleva with Skhokho and TymeBank',
          }
        ],
      }
    },
}
</script>
<style scoped>
h5{
    font-weight: normal;
    font-size: 30px;
}
h3{
    font-size: 30px;
}
h4{
    font-weight: normal;
    font-size: 20px;
}
#rect{
    background-color: #D100C9;
}
#caseStudies{
    color: white;
}
</style>