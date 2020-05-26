<template>

<div id="cta-bg">

<div class="container">

    <div>
        <h4>Simplify how your team <span>works today.</span></h4>
    </div>

    <div>
        <a class="ctaButton white" href="#">Get Started</a>
    </div>

</div>

</div>

</template>

<script>
export default {
  name: 'CTA',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/css/core.scss";

#cta-bg {

    padding:70px 0;
    background: #ff5722e0 url(../assets/img/bg-simplify-section-desktop.svg);
}

.white {
    background:white; 
    color:$orange;
}

.container div {
    text-align: center;
}

.container div a {
        margin-top: 20px;
    display: block;
    margin: 20px auto;
    width: fit-content;
}

h4 {
    text-align: center;
    font-size: 30px;
}

.white:hover {
    background:white;
}

@media screen and (min-width: 800px) {

.container {
display: flex;
}

.container div {
    flex:1;
}

.container div a {
        display: initial;
    width: inherit;
}

.container div:last-of-type {
    text-align:right;
    margin-top:30px;
    padding-right:30px
}

h4 span {
    display:block;
}

h4 {
    text-align:left;
}


}


</style>
