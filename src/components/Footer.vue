<template>

<footer>

    <div class="container">

        <div>
           <logo :footer="footer" />
           <Social />
        </div>


        <div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">Products</a></li>
                <li><a href="#">About Us</a></li>
            </ul>
        </div>

        
        <div>
             <ul>
                <li><a href="#">Careers</a></li>
                <li><a href="#">Community</a></li>
                <li><a href="#">Privacy Policy</a></li>
            </ul>
        </div>

        
        <div>
            <input type="email" id="email" name="email" placeholder="Updates in your inbox...">
            <input type="submit" value="Go" id="submit">
        </div>

    </div>

</footer>

</template>

<script>
import Logo from './Logo.vue';
import Social from './Social.vue';

export default {
  name: 'Footer',
  components: {
      Logo,
      Social
  },

  data() {
    return {
      footer: true
    };
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/css/core.scss";

footer {
    background:$black;
    padding:50px 0;
}


ul {
    margin:0px;
}

ul li {
    margin-bottom:10px;
}

ul li a {
    color:$white;
    text-decoration:none
}

ul li a:hover {
    text-decoration: underline;
}

#email {
    padding: 10px 20px 10px 20px;
    border: 0;
    border-radius: 30px;
    margin-right: 10px;
}

#submit {

   padding: 10px 20px 10px 20px;
    border: 0;
    border-radius: 30px;
    color:$white;
    background:$orange;

}

ul {
    padding-left:0
}

.container div {
    text-align: center;
    margin-bottom:30px;
}


@media screen and (min-width: 800px) {

    ul {
    padding-left:initial;
}

.container div {
    text-align: left;
    margin-bottom:0px;
}

.container {
     display:flex;
}

.container div {
    flex:1;
}

}

</style>
