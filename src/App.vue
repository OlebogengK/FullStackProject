<template>
  <header>
    <div class="d-none d-md-flex justify-space-between mx-16">
      <div>
        <v-img
          height="90"
          width="90"
          src="/logo.svg"
        >
        </v-img>
      </div>
      <div>
        <ul class="d-md-flex">
          <li class="mx-2 my-6 pa-2 font-weight-bold"><router-link to="/" class="routerLink">Services</router-link></li>
          <li class="mx-2 my-6 pa-2 font-weight-bold"><router-link to="/" class="routerLink">Industries</router-link></li>
          <li class="mx-2 my-6 pa-2 font-weight-bold"><router-link to="/" class="routerLink">Cases</router-link></li>
          <li class="mx-2 my-6 pa-2 font-weight-bold"><router-link to="/" class="routerLink">Contact</router-link></li>
        </ul>
      </div>
      <div>
        <v-btn class="mt-6" rounded="xl" id="letsTalk">Lets Talk</v-btn>
      </div>
      </div>
      <div class="d-flex justify-space-between d-md-none">
        <router-link to="/" class="routerLinkLogo">
          <v-img
            height="90"
            width="90"
            src="/logo.svg"
          >
          </v-img>
        </router-link>
        <div class="d-flex d-md-none">
          <v-app-bar-nav-icon  color="white" v-model="appBar" class="d-flex d-md-none mt-6" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        </div>
      </div>
      <v-layout>
        <v-navigation-drawer v-model="drawer" location="left" temporary class=" d-flex d-md-none"  absolute="true">
          <v-list :items="items"></v-list>
        </v-navigation-drawer>
      </v-layout>
  </header>
<router-view/>
</template>

<script>
import Hero from './components/HeroComponent.vue'
export default{
  components:{
        Hero
  },
  data: () => ({
    drawer: false,
    windowWidth:null,
    group: null,
    items: [
      {
        title: 'Services',
        value: 'Services',
      },
      {
        title: 'Industries',
        value: 'Industries',
      },
      {
        title: 'Cases',
        value: 'Cases',
      },
      {
        title: 'Contact',
        value: 'Contact',
      },
    ],
  }),
  watch: {
    group() {
      this.drawer = false
    },
  }
}

</script>

<style scoped>
#letsTalk{
  color: #70259B;
}
header{
  background: #70259B;
}
li{
  list-style-type:none;
  color: white;
  text-shadow: black 0px 0px 2px;
}
#logo{
  font-family: 'Work Sans', sans-serif;
  font-weight: bold;
  font-size: xx-large;
}
.routerLink{
   text-decoration: none;
   color: white;
}
.routerLink:hover {
text-decoration: underline;
text-decoration-thickness: 3px;
}
.routerLinkLogo{
text-decoration: none;
color: white;
}
#socials:hover{
opacity: 0.5;
}
#app{
height: max-content;
}


</style>
