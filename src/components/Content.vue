<template>

<div id="bg">
    
    <div class="container">

        <div>
            <h2>Whats different about <span>Manage?</span></h2>
            <p class="greyText middleP">Manage provides all the functionality your team needs, without the complexity. Our software is tailor-made for modern digital product teams. </p>

        </div>

        <div>
            <ul>
                <li>
                    <span class="bubble">1</span>
                    <h3>Track company-wide progress</h3>
                    <span class="greyText">See how your day-to-day tasks fit into the wider vision. Go from tracking progress at the milestone level all the way done to the smallest of details. Never lose sight of the bigger picture again.</span>
                </li>

                <li>
                    <span class="bubble">2</span>
                    <h3>Advanced built-in reports</h3>
                    <span class="greyText">Set internal delivery estimates and track progress toward company goals. Our customisable dashboard helps you build out the reports you need to keep key stakeholders informed.</span>
                </li>

                <li>
                    <span class="bubble">3</span>
                    <h3>Everything you need in one place</h3>
                    <span class="greyText">Stop jumping from one service to another to communicate, store files, track tasks and share documents. Manage offers an all-in-one team productivity solution.</span>
                </li>

            </ul>
        </div>

    </div>

    <div class="testimonials">
        
        <h2>What they’ve said</h2>

        <div class="test-container">

            <div>
                <img src="../assets/img/avatar-anisha.png" alt="avatar">
                <strong>Anisha Li</strong>
                <p class="greyText">“Manage has supercharged our team’s workflow. The ability to maintain visibility on larger milestones at all times keeps everyone motivated.”</p>
            </div>

            <div>
                <img src="../assets/img/avatar-ali.png" alt="avatar">
                <strong>Ali Bravo</strong>
                <p class="greyText">“We have been able to cancel so many other subscriptions since using Manage. There is no more cross-channel confusion and everyone is much more focused.”</p>
            </div>

            <div>
                <img src="../assets/img/avatar-richard.png" alt="avatar">
                <strong>Richard Watts</strong>
                <p class="greyText">  “Manage allows us to provide structure and process. It keeps us organized and focused. I can’t stop recommending them to everyone I talk to!"</p>
            </div>

        </div>

        <a class="ctaButton" href="#">Get Started</a>

    </div>

</div>

</template>

<script>
export default {
  name: 'Content',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../assets/css/core.scss";

#bg {
    background-image: url(../assets/img/bg-tablet-pattern.svg);
    background-repeat: no-repeat;
    background-position: -65% 150%;
 
}

.container {
    display:flex;
    flex-flow:column;
}

.container div {
flex:1;
}

p {
    max-width: 500px;
    width: 100%;
    margin-bottom:30px;
    
}

.middleP {
    max-width: 400px;
    width: 90%;
    margin: 20px auto 30px auto;
    text-align: center;
}


h3 {
    margin: 0px 0px 10px 0px;
    color: $blue;
    background: #fff0ec;
    text-align: center;
    font-size: 16px;
    padding-top: 5px;
    padding-bottom: 5px;
}

h2 {
    font-size: 37px;
    text-align: center;
}

ul {
position:relative;
padding:0 10px;
}

ul li {
    list-style: none;
    margin-bottom:25px;
}

ul li .bubble {
    font-size: 12px;
    position: absolute;
    left: 5px;
    background:$orange;
    padding: 7px;
    padding-left: 20px;
    padding-right: 20px;
    color: white;
    border-radius: 30px;
    font-weight: bold;
}


.testimonials {
padding-bottom:50px;
}

.testimonials h2 {
    text-align: center;
    padding:60px 0px;
}

.test-container {
    margin:20px 0px;
}

.test-container div {
    flex:1;
    text-align: center;
    padding: 0px 20px;
}

.test-container img {
    display: block;
    margin: 20px auto 20px auto;
    width: 100px;
}

.ctaButton {
    display: block;
    width: fit-content;
    margin: auto;
    text-align: center;
}

@media screen and (min-width: 800px) {

    h3 {
    margin:0px 0px 10px 0px;
    font-size: 22px;
    color:$blue;
    text-align: left;
    background:none;
    padding:0
}

ul {
    padding:0px 0px 0px 40px;
}

ul li .bubble
{
    left:-25px;
}

.container {
     flex-flow:initial;
}

.test-container {
    display:flex;
}

h2 {
    text-align: left;
}

h2 span {
    display:block;
}


}

</style>
