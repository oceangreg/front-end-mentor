<template>

  <header id="mob">

    <div class="container">

        <div class="logo flexBlockSmall">

            <logo :header="header" />

        </div>

        <nav class="flexBlockLarge">

        <div id="mobdrop" v-show='toggle'>
          <ul>
            <li><a href="#">Pricing</a></li>
            <li><a href="#">Product</a></li>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Careers</a></li>
            <li><a href="#">Community</a></li>
          </ul>
        </div>

        </nav>

        <div class="cta flexBlockSmall">

          
          <span id="hamburger" @click='toggle = !toggle'>
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="18"><g fill="#242D52" fill-rule="evenodd"><path d="M0 0h25v4H0zM0 7h25v4H0zM0 14h25v4H0z"/></g></svg>
          </span>

            <a class="ctaButton" href="#">Get Started</a>

        </div>

      </div>

  </header>

</template>

<script>
import Logo from './Logo.vue';



export default {
  name: 'Header',
  components: {
    Logo
  },
  data() {
    return {
      header: true,
      toggle: false
    };
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

// Colours
@import "../assets/css/core.scss";

header {
margin-top: 20px;
}

nav {

}

nav ul {
  margin:0;
}

nav li {
    display: block;
}

nav li a {
  text-decoration: none;
  display: block;
  margin: 0px 15px 0px 15px;
  color:$blue;
  padding:10px 0;
}

nav li a:hover {
  text-decoration: underline;
}

.container {
  display:flex
}

.flexBlockSmall {
  flex: 0.5;
}

.flexBlockSmall:last-of-type {
  text-align:right;
}

.flexBlockLarge {
  flex: 1.5;
  text-align:center;
}

#mobdrop {
    width: 100%;
    position: absolute;
    left: 0;
    top: 50px;
}

#mobdrop ul {
    padding-left: 0;
    max-width: 90%;
    margin: auto;
    background: $white;
    box-shadow: 0px 18px 32px #242d5224;
}

#hamburger {
  display: block;
  padding-right: 20px;
}

.ctaButton {
  display:none
}

.logo {
  padding-left: 20px;
}

@media screen and (min-width: 800px) {

.logo {
  padding-left: 0;
}

#mobdrop  {
  display:block!important;
}

.ctaButton {
display:initial;
}

header {
margin-top: 40px;
}

#hamburger {
  display: none;
}

#mobdrop {
    position: inherit;
    top: 0;
    left: inherit;
}

#mobdrop ul {
  margin:initial;
  background:none;
  padding:initial;
  box-shadow: none;
  max-width: inherit;
}

#mobdrop ul li {
  display: inline-block;
}

#mobdrop ul li a {
  padding:0
}




}

</style>
