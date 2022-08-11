<template>
  <div class="support">
    <appHeader></appHeader>
    <div class="container-fluid">
        <div class="row">
            <div class="col-md-5">
                <div class="superHeader"><b>Contact Us</b></div>
            </div>

            <div class="col-md-7 support-column"></div>
        </div>

        <div class="row flex-column-reverse flex-md-row">
            <div class="col-md-5">
                <div class="rowddd">
                    <div class="address">
                        <h2><b>Corporate Head Office</b></h2>
                        <h3><b>Head Office Address</b></h3>
                        <h3>14, ORANGE GATE, PLAMER STREET, OLUYOLE ESTATE IBADAN, IBADAN, OYO STATE, NIGERIA</h3>
                    </div>
                </div>

                <div class="rowddd">
                    <div class="contact">
                        <h2><b>Checkretail Connect</b></h2>
                        <h3><a href="tel:+234 903 771 6931">Tel: +234 903 771 6931</a></h3>
                        <h3><a href="tel:08149734622">Tel: 08149734622</a></h3>
                        <h3><a href="tel:+234 808 462 2379">Tel: +234 808 462 2379</a></h3>
                    </div>
                </div>

                <div class="rowddd">
                    <div class="contact">
                        <h2><b>Social Media</b></h2>
                        <ul>
                            <li><a href="https://www.facebook.com/CheckRetail-109076205144232/"><img src="../assets/icons/icons8-facebook.svg"></a></li>
                            <li><a href="https://instagram.com/check.retail?igshid=YmMyMTA2M2Y="><img src="../assets/icons/icons8-instagram.svg"></a></li>
                            <li><a href="https://www.youtube.com/channel/UCA2tE3-Fi8OEopE28Se_e6g"><img src="../assets/icons/icons8-youtube.svg"></a></li>
                            <!--<li><img src="../assets/icons/icons8-linkedin.svg"></li>
                            <li><img src="../assets/icons/icons8-twitter.svg"></li>-->
                        </ul>
                        <h3></h3>
                    </div>
                </div>
            </div>
            <div class="col-md-7 support-column">
                <div class="support-container">
                    <img src="../assets/images2/support5.jpg" class="desktop-img">
                    <img src="../assets/images2/support5.2.jpg" class="mobile-img">
                    <!--<div class="superHeader-mobile"><b>Contact Us</b></div>-->
                </div>
            </div>
        </div>

    </div>
    <footerLinks></footerLinks>


  </div>
</template>

<script>

import appHeader from '../components/headerNav.vue';
//import qrSection from '../components/qrSection.vue';
//import oneApp from '../components/oneApp.vue';
//import trustedBy from '../components/trustedBy.vue';
import footerLinks from '../components/linksFooter.vue';

//import gsap from 'gsap'

export default {
  name: 'HomeView',
  components: {
    //HelloWorld,
    appHeader,
    //qrSection,
    //oneApp,
    //trustedBy,
    footerLinks
  }

}
</script>

<style scoped>
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');

.support {
    margin: 0%;
    padding: 0%;
    overflow-x: hidden;
}
a {
    color: black;
    text-decoration: none;
}
.superHeader {
    color: black;
    font-family: 'Euclid Circular A';
    font-size: 50px;
    font-weight: 500px;
    text-align: left;
    margin-left: 120px;
    margin-top: 100px;
    margin-bottom: 80px;
}
.address, .contact {
    text-align: left;
    color: black;
    font-family: 'Euclid Circular A';
    margin-left: 120px;
    margin-top: 30px;
}
.address h2 {
    /*font-weight: 300;*/
    font-size: 30px;
    line-height: 45px;
    margin-bottom: 40px;
}
.address h3, .contact h3 {
    font-weight: 300;
    font-size: 20px;
    line-height: 30px;
    width: 350px;
}
.contact ul li {
    list-style: none;
    display: inline-block;
}
.contact ul {
    margin-left: -40px;
}
.support-container {
    width: 600px;
    height: 800px;
    margin-left: 100px;
    margin-top: -200px;
    transform: scale(0.8);


}
.support-container img {
    width: 100%;
    height: 100%;
    border-radius: 30px;
    animation-name: fade;
    animation-duration: 2s;
    transition: 0.4s ease;
}
.mobile-img {
    display: none;
}
.support-column {
    background: #FFF6FF;
}
@keyframes fade {
    from {opacity: 0;}
    to {opacity: 1;}
}

@media screen and (max-width: 800px) {
    .support {
        margin: 0px;
        padding: 0px;
    }
    /*.container {
        padding-right: 20px;
    }*/
    .superHeader {
        margin-left: -30px;
        margin-bottom: 10px;
        font-size: 30px;
        /*position: absolute;*/
        color: rgb(255, 255, 255);
        background: #000000;
        margin-top: 10px;
        width: 200%;
        padding-left: 50px;
    }
    .address, .contact {
        margin-left: 20px;
    }
    .address h2 {
        /*width: 300px;*/
        line-height: 45px;
    }
    .address h3, .contact h3 {
        /*width: 300px;*/
        padding-right: 30px;
    }
    .support-container {
        transform: scale(0.9);
        margin-top: 0px;
        margin-top: -30px;
        margin-left: -130px;
        height: 400px;
    }
    .support-container img {
        position: relative;
    }
    .mobile-img {
        display: block;
    }
    .desktop-img {
        display: none;
    }
    /*.superHeader-mobile {
        margin-left: 135px;
        margin-bottom: 30px;
        font-size: 40px;
        position: absolute;
        color: rgb(255, 255, 255);
        margin-top: -730px;
        text-align: left;
        font-family: 'Euclid Circular A';
    }*/
}



</style>
