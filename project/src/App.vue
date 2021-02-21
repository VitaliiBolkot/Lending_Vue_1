<template>
  <div id="app">
      <NavBar />
      <Home />
      <About id="about" />
      <Works id="works"/>
      <Services id="services"/>
      <Prices id="prices"/>
      <BackVideo id="blog"/>
      <TestImonials />
      <Clients id="clients" />
      <Blog />
      <ContactUs id="contact"/>
      <FindUs />
      <Footer/>
  </div>
</template>

<script>
  import NavBar from '@/components/NavBar'
  import About from '@/components/About'
  import Home from '@/components/Home'
  import Works from '@/components/Works'
  import Services from '@/components/Services'
  import Prices from '@/components/Prices'
  import BackVideo from '@/components/BackVideo'
  import TestImonials from '@/components/TestImonials'
  import Clients from '@/components/Clients'
  import Blog from '@/components/Blog'
  import ContactUs from '@/components/ContactUs'
  import FindUs from '@/components/FindUs'
  import Footer from '@/components/Footer'
  export default{

    components:{
      NavBar,
      About,
      Home,
      Works,
      Services,
      Prices,
      BackVideo,
      TestImonials,
      Clients,
      Blog,
      ContactUs,
      FindUs,
      Footer
    }
  }
  
</script>

<style lang="scss">
  
    @import "~materialize-css/dist/css/materialize.min.css";
    #app{
      display: flex;
    flex-direction: column;
    }

   

</style>
