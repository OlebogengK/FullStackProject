<template>
  <Hero />
  <WhatWeDo />
  <CaseStudies />
  <TrustedPartners />
  <Contact />
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/HeroComponent.vue'
import WhatWeDo from '@/components/WhatWeDo.vue'
import CaseStudies from '@/components/CaseStudies.vue'
import TrustedPartners from '@/components/TrustedPartners.vue'
import Contact from '@/components/ContactUs.vue'
export default {
  name: 'HomeView',
  components: {
    Hero,
    WhatWeDo,
    CaseStudies,
    TrustedPartners,
    Contact
  }
}
</script>
