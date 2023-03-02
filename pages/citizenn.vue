<template>
  <div>
        <HeaderPage />
        <!-- <nuxt-child /> -->
        <InforCitizen/>
        <FooterPage />

       
    </div>
</template>
    
<script>
import HeaderPage from '~/components/Header/HeaderPage.vue'
import Logo from '~/components/Logo.vue'
import FooterPage from '~/components/Footer/FooterPage.vue'
export default {
    components: {
        HeaderPage,
        Logo,
        FooterPage,

    },
}
</script>
    
<style scoped>

</style>