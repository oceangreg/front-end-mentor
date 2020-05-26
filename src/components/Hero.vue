<template>

  <div class="hero">

      <div class="container">

        <div>
            <h1>Bring everyone 
                <span>together to build</span> 
                <span> better products.</span>
            </h1>
            <p class="greyText">Manage makes it simple for software teams to plan day-to-day tasks while keeping the larger team goals in view.</p>
            <a href="#" class="ctaButton">Get Started</a>
        </div>

      <div>

          <img src="../assets/img/illustration-intro.svg" alt="hero ullustration" >

      </div>

  </div>

  </div>

</template>

<script>
export default {
  name: 'Hero',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/css/core.scss";

.hero {
    padding:40px 0px 40px 0px;
}

.hero img {
    width:100%
}

p {
    max-width: 400px;
    width: 90%;
    margin:20px auto 30px auto;

}

h1 {
    font-size: 36px;
    line-height: 45px;
    margin:0;
    color:$blue;
}

.container {
    display:flex;
    flex-flow: wrap;
}

.container div {
    order:2;
    text-align:center;
}

.container div:last-of-type {
    order:1;
}

@media screen and (min-width: 800px) {

    .hero {
    padding:90px 0px 40px 0px;
}

.container div {
    flex:1;
    text-align:left
}

.container div:last-of-type {
    order:2;
}

h1 {
    font-size: 54px;
    line-height: 65px;
}

h1 span {
    display:block;
}

p {
    margin:30px 0;
    width: 100%;

}

}

</style>
