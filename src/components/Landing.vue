<template>
<div>
  <Header></Header>
  <Hero></Hero>
  <Content></Content>
  <CTA></CTA>
  <Footer></Footer>
</div>
</template>

<script>
import Header from './Header.vue';
import Hero from './Hero.vue'
import Content from './Content.vue'
import CTA from './CTABanner.vue'
import Footer from './Footer.vue'

export default {
  name: 'Landing',
  components: {
    Header,
    Hero,
    Content,
    CTA,
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
