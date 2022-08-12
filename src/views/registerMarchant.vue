<template>
  <div class="register">
    <div class="color"></div>
    <!--<h1>This is an about page</h1>-->
    <appHeader></appHeader>

    <div class="container-fluid">
        <div class="grid-contain-1 row flex-column-reverse flex-md-row">
                <div class="first-container col-md-6">

                    <h3 class="we-are-obsessed slide-in">We are obsessed about making things work for you and your business!</h3>
                    <h3 class="how-we-built slide-in-delay">How we built the solution that works for you</h3>

                    <h3 class="our-expert">Our expert engineers use technically driven deep algorithm to power our QR code system which is the anchor of  our innovation.
                    The QR code technology is a faster way to send and receive data which eliminates every form of failure and disconnection in your transactions. </h3>
                </div>

                <div class="col-md-6">
                    <div class="modal-content fade-up" id="form1">
                        <form action="https://formsubmit.co/hello.paddle@gmail.com" method="POST">
                            <!--<h2 @click="form1 = !form1">+</h2>-->
                            <h1>Drop your details, we will surely reach back!</h1>
                            <input type="email" name="Email" placeholder="Email" class="email-input" required><br>
                            <input type="tel" name="Phone-number" placeholder="Phone number eg: 08180334573"  required><br>
                            <input type="text" name="Company-name" placeholder="Company name" required><br>
                            <input type="submit" value="Contact me!" class="submit-btn">
                        </form>
                    </div>
                </div>

        </div>
    </div>

    <div class="row row2register">

        <aos-vue animation="" class="col-md-6">
            <aos-vue animation="fade-right">
                <img src="../assets/images/Vector-34.png" class="table">
            </aos-vue>
            <img src="../assets/images/Vector-34.png" class="table2">

        </aos-vue>



        <aos-vue animation="fade-left" class="col-md-6">
            <div class="number1">
                <img src="../assets/pic1/pic2/01.png" class="num1"><br>
                <p class="restaurant-class">Restaurant</p>
                <!--<div class="restaurant-block">
                    <img src="../assets/pic1/pic2/Rectangle-64.png" class="restaurant-box">
                    <img src="../assets/pic1/pic2/Restaurant.png" class="restaurant">
                </div>-->


                <h3 class="trying-to">Trying to sell to tens of customers at the same time is tiring, Our app will save you!</h3>
                <h3 class="you-are-here">You are here because the future matters. We  thought  of what you need and expressed it in this beautiful piece of technology.</h3><br><br>

                <ul class="list1">
                    <li><img src="../assets/images/check-pink.png" class="check"><p class="list-text">Up to 30% increase sales</p></li><br>
                    <li><img src="../assets/images/check-pink.png" class="check"><p class="list-text">Quick menu look-up for customer</p></li><br>
                    <img src="../assets/images/check-pink.png" class="check"><li><p class="list-text list3">No more change and POS delay</p></li><br><br>

                    <a href="#form1"><button @click="form1 = !form1" class="btn-1">Start Now</button></a>


                </ul>
            </div>
        </aos-vue>
    </div>


    <!--<transition name="form" mode="out-in" appear>
        <div class="modal-row" id="form1" v-show="form1">
            <div class="modal-content">
                <form action="https://formsubmit.co/hello.paddle@gmail.com" method="POST">
                    <h2 @click="form1 = !form1">+</h2>
                    <h1>Drop your details, we will surely reach back!</h1>
                    <input type="email" name="Email" placeholder="Email" class="email-input" required><br>
                    <input type="number" name="Phone-number" placeholder="Phone number eg: 08180334573" required><br>
                    <input type="text" name="Company-name" placeholder="Company name" required><br>
                    <input type="submit" value="Contact me!" class="submit-btn">
                </form>
            </div>
        </div>
    </transition>-->


    <div class="row row2register">
        <!--<>-->
            <aos-vue animation="fade-right" class="col-md-6">
            <div class="number2">
                <img src="../assets/pic1/pic2/02.png" class="num1"><br>
                <p class="supermarket-class">Supermarket</p>
                <!--<div class="supermarket-block">
                    <img src="../assets/pic1/pic2/Rectangle-69.png" class="restaurant-box">
                    <img src="../assets/pic1/pic2/Supermarket.png" class="restaurant ">
                </div>-->


                <h3 class="trying-to">Trying to sell to tens of customers at the same time is tiring, Check will save you!</h3>
                <h3 class="you-are-here">You are here because the future matters. We  thought  of what you need and expressed it in this beautiful piece of technology.</h3><br><br>

                <ul class="list1">
                    <li><img src="../assets/images/check-green.png" class="check"><p class="list-text">Up to 30% increase sales</p></li><br>
                    <li><img src="../assets/images/check-green.png" class="check"><p class="list-text">Quick menu look-up for customer</p></li><br>
                    <li><img src="../assets/images/check-green.png" class="check"><p class="list-text list6">No more change and POS delay</p></li><br><br>

                     <a href="#form1"><button @click="form1 = !form1">Start Now</button></a>

                </ul>
            </div>
        </aos-vue>
        <!--</>-->


        <aos-vue animation="fade-left" class="col-md-6">
            <aos-vue animation="fade-in">
                <img src="../assets/images/Vector-33.png" class="woman-with-phone-pic">
            </aos-vue>
        </aos-vue>
    </div>





    <oneApp></oneApp>
    <trustedBy></trustedBy>
    <footerLinks></footerLinks>
  </div>
</template>

<script>

import appHeader from '../components/headerNav.vue';
import oneApp from '../components/oneApp.vue';
import trustedBy from '../components/trustedBy.vue';
import footerLinks from '../components/linksFooter.vue';

export default {
  name: 'RegisterMarchant',
  components: {
    appHeader,
    oneApp,
    trustedBy,
    footerLinks
  },
  data() {
    return {
        form1: false,
        form2: false
    }
  }
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Poppins:wght@300;500;600&display=swap');
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');

* {
    margin: 0%;
    padding: 0%;
}
.container-fluid {
    margin: 0%;
    padding: 0%;
    /*transform: translateY(-200px);*/
}
.register {
    background: #fff;
    overflow-x: hidden;
    font-family: 'Euclid Circular A';
}
.first-container {
    text-align: centers;
    height: 800px;
    /*transform: translateY(-275px);*/
    /*margin-top: -270px;*/
    position: relative;
    margin-bottom: 200px;
}
.color {
    background-color: #FFF6FF;
    /* transform: translateY(-80px); */
    height: 350px;
    position: absolute;
    width: 100%;
}
.we-are-obsessed {
    position: relative;
    font-family: 'poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 60px;
    line-height: 70px;
    text-align: center;
    letter-spacing: -0.05em;
    /*with was formally 1000px */
    width: 550px;

    margin-top: 182px;
    position: relative;
    left: 50%;
    transform: translateX(-44%);
    color: black;
    font-family: 'Euclid Circular A';

    /* margin-left: 131px; */
    text-align: left;
}
.how-we-built {
    font-family: 'poppins';
    text-align: center;
    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 30px;
    text-align: left;
    margin-top: 91px;
    color: black;

    margin-left: 90px;
}
.our-expert {
    font-family: 'poppins';
    /*text-align: center;*/
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 25px;
    text-align: left;
    width: 561px;
    position: relative;
    left: 50%;
    transform: translateX(-44%);
    margin-top: 26px;
    color: black;
}



.table {
    margin-left: 80px;
    /*transform: scale(0.78) scaleY(1.05) ;*/
    /*margin-top: -360px;*/
    margin-bottom: 204px;

    width: 520px;
    height: 703px;
}
.table2 {
    margin-left: 80px;
    margin-bottom: 204px;

    width: 520px;
    height: 703px;
    display: none;
}
.woman-with-phone-pic {
    margin-left: 0px;
    margin-bottom: 204px;

    width: 560px;
    height: 743px;
}
.move-container {
    transform: translateY(-1070px);
}

.num1{
    /*transform: translateX(-200px);*/
    float: left;
    margin-left: 50px;
}
.restaurant-class {
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 500;
    font-size: 30px;
    line-height: 38px;
    /* identical to box height */

    display: flex;
    align-items: center;
    text-align: center;

    color: #9D5259;
    padding: 0px 34px 0px 34px;
    width: 231px;
    height: 50px;
    /*left: 821px;
    top: 958px;*/

    background: #F6E7F6;
    border-radius: 5px;
    margin-top: 27px;
    margin-left: 50px;
}

.supermarket-class {
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 500;
    font-size: 30px;
    line-height: 38px;
    /* identical to box height */

    display: flex;
    align-items: center;
    text-align: center;

    color: #58836B;
    padding: 0px 17px 0px 17px;
    width: 231px;
    height: 50px;
    /*left: 821px;
    top: 958px;*/

    background: #C1EDD4;
    border-radius: 5px;
    margin-top: 27px;
    margin-left: 50px;
}
/*.restaurant-box {
    transform: translateY(20px) translateX(-30px);
}
.restaurant-block {
    float: left;
    margin-top: 5px;
    margin-left: -7px;
}*/
/*.supermarket-block {
    float: left;
    margin-top: 5px;
    margin-left: -15px;
}
.restaurant {
    transform: translateY(20px) translateX(-230px);
}*/
.number1 {
    /*transform: translateY(-260px);*/
    transform: translateY(-5px);
}
.btn-1 {
    /*transform: translateY(-50px);*/
    margin-top: -50px;
}
.number2 {
    margin-left: 50px;
}
.trying-to {
    font-family: 'poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 45px;
    line-height: 50px;
    letter-spacing: -0.05em;
    text-align: left;
    width: 580px;
    transform: translateY(30px) translateX(50px);
    margin-bottom: 40px;
    color: black;
    font-family: 'Euclid Circular A';
}
.you-are-here {
    font-family: 'poppins';
    text-align: left;
    transform: translateY(40px) translateX(50px);
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 25px;
    width: 540px;
    font-family: 'Euclid Circular A';
}
.check {
    width: 38px;
    height: 30px;
}
ul {
    text-align: left;
    margin-top: 51px;
    margin-left: 50px;

    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 25px;
    color: #000000;
    font-family: 'Euclid Circular A';
}
li {
    list-style: none;

}
.list-text {
    margin-left: 10px;
    display: inline-block;
}
.list3 {
    transform: translate(40px, -30px);
}
.list6 {
    transform: translate(0px, 0px);
}
button {
    width: 294px;
    height: 77px;
    background: #40BC77;
    color: #fff;
    border: none;
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 500;
    font-size: 30px;
    line-height: 38px;
    transition: all 0.4s ease;
    border-radius: 10px;
}
button:hover {
    transform: scale(1.05);
    transition: all 0.4s ease;
    opacity: 0.9;
}


@keyframes slide-in {
    from {
        transform: translateX(-1000px);
        opacity: 0;
        };
    to {
        transform: translateX(0);
        opacity: 1;
    }
}

@keyframes slide-from-right {
    from {
        transform: translateX(1000px);
        opacity: 0;
        };
    to {
        transform: translateX(0);
        opacity: 1;
    }
}
@keyframes fade-up {
    0% {
        transform: translateY(455px);
        opacity: 0;
        transition: all 0.4s ease;
        };
    30% {
        transform: translateY(140px);
        opacity: 0.7;
        transition: all 0.4s ease;
        };
    70% {
        transform: translateY(55px);
        opacity: 0.9;
        transition: all 0.4s ease;
        };
    100% {
        transform: translateY(0px);
        opacity: 1;
        transition: all 0.4s ease;
        }
}
/*.slide-from-up {
    animation: slide-from-up 1.5s;
}*/
.slide-in {
    animation: slide-in 1.5s;
}
.slide-in-delay {
    animation: slide-in 1.9s;
}
.slide-from-right {
    animation: slide-from-right 1.5s;
}
.fade-up {
    animation-name: fade-up;
    animation-duration: 1.5s;
    transition: all 0.4s ease;
}
.modal-row {
    width: 100%;
    height: 200%;
    background: rgba(0, 0, 0, 0.75);
    /*position: absolute;*/
    position: relative;
    top: 0;

    display: flex;
    justify-content: center;
    align-items: center;
}

/*.modal-content {
    position: absolute;
    width: 759px;
    height: 970px;
    top: 223px;

    background: #FFFFFF;
    border-radius: 20px;
    padding: 77px;
    text-align: left;
}
.modal-content h2 {
    float: right;
    transform: rotate(45deg);
    margin-top: -55px;
    margin-right: -22px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 40px;
    color: #464646;
    cursor: pointer;
}
.modal-content h1 {
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 600;
    font-size: 60px;
    line-height: 70px;

    display: flex;
    align-items: center;
    letter-spacing: -0.05em;

    color: #464646;
    width: 514px;
}
.modal-content input {
    width: 100%;
    height: 50px;
    border: none;
    border-bottom: 0.5px solid #000000;
    padding: 85px 0px 16px px;
    margin-bottom: 49px;
    padding-bottom: 30px;

    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 70px;
    letter-spacing: -0.05em;

    color: #464646;
    transition: all 0.4s ease;
}
.modal-content .email-input {
    margin-top: 40px;
}
.modal-content .submit-btn {
    color: rgb(255, 255, 255);
    background: #EB001B;
    padding: 0px;
    margin-top: 83px;
    height: 85px;
    border-radius: 10px;
    border: none;

    font-style: normal;
    font-weight: 500;
    font-size: 36px;
    line-height: 70px;


    align-items: center;
    letter-spacing: -0.05em;

}
.modal-content input:focus {
   border: none;
   border: 2px solid #EB001B;
   outline: none;
   border-radius: 8px;
   padding: 10px;
   transform: scale(1.02);
   height: 60px;
   transition: all 0.4s ease;
}*/




.modal-content {
    position: relative;
    width: 659px;
    height: 770px;
    top: 123px;

    background: #FFFFFF;
    border-radius: 20px;
    padding: 47px;
    text-align: left;
    border: none;
    transition: all 0.4s ease;
}
.modal-content h2 {
    float: right;
    /*text-align: right;*/
    transform: rotate(45deg);
    margin-top: -55px;
    margin-right: -22px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 40px;
    color: #464646;
    cursor: pointer;
}
.modal-content h1 {
    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 600;
    font-size: 60px;
    line-height: 70px;
    /* or 117% */

    display: flex;
    align-items: center;
    letter-spacing: -0.05em;

    color: #464646;
    width: 514px;
}
.modal-content input {
    width: 100%;
    height: 50px;
    border: none;
    border-bottom: 0.5px solid #000000;
    padding: 25px 0px 12px px;
    margin-bottom: 24px;
    padding-bottom: 10px;

    font-family: 'Euclid Circular A';
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 70px;
    /*display: flex;
    align-items: center;*/
    letter-spacing: -0.05em;

    color: #464646;
    transition: all 0.4s ease;
}
.modal-content .email-input {
    margin-top: 40px;
}
.modal-content .submit-btn {
    color: rgb(255, 255, 255);
    background: #EB001B;
    /*height: 70px;*/
    padding: 0px;
    margin-top: 40px;
    height: 85px;
    border-radius: 10px;
    border: none;

    font-style: normal;
    font-weight: 500;
    font-size: 36px;
    line-height: 70px;
    /* or 194% */

    align-items: center;
    letter-spacing: -0.05em;

}
.modal-content input:focus {
    /*border: 2px solid #EB001B;*/
   border: none;
   border: 2px solid #EB001B;
   outline: none;
   border-radius: 8px;
   padding: 10px;
   transform: scale(1.02);
   height: 60px;
   transition: all 0.4s ease;
}






.form-enter-from {
  opacity: 0;
  transform: translateY(100px);
  /*transform: scaleX(0);*/
}
.form-enter-to {
  opacity: 1;
  transform: translateX(0);
  /*transform: scaleX(1);*/
}
.form-enter-active {
  transition: all 0.8s ease;
}
.form-leave-from {
  opacity: 1;
  transform: translateX(0);
   /*transform: scaleX(1);*/
}
.form-leave-to {
  opacity: 0;
  transform: translateY(100px);
  /*transform:scaleX(0);*/
}
.form-leave-active {
  transition: all 0.8s ease;

}



@media screen and (max-width: 800px) {
    .first-container {
        text-align: left;
        height: 1200px;
        margin-left: 0%;
        margin-bottom: 20px;
    }
    .we-are-obsessed {
        font-size: 45px;
        line-height: 50px;
        text-align: left;
        width: 350px;
        margin-left: 20px;
        left: 0%;
        transform: translateX(0%);
        margin-top: 40px;
        /*transform: translateX(-55%);*/
    }
    .how-we-built {
        text-align: left;
        margin-left: 20px;
        width: 350px;
        margin-top: 30px;
    }
    .our-expert {
        text-align: left;
        margin-left: 20px;
        width: 310px;
        left: 0%;
        transform: translateX(0%);
    }
    .color {
        /* transform: translateY(-80px); */
        height: 450px;
        /*position: fixed;*/
    }
    .table {
        margin-left: 0px;
        margin-bottom: 204px;
        margin-top: -400px;
        width: 320px;
        /*height: 523px;*/
        height: 463px;
        display: none;
    }
    .table2 {
        display: inline-block;
       margin-left: 0px;
        margin-bottom: 204px;
        margin-top: -500px;
        width: 320px;
        /*height: 523px;*/
        height: 463px;
    }
    .woman-with-phone-pic {
        margin-left: 0px;
        margin-bottom: 84px;

        width: 320px;
        height: 463px;
    }

    .num1{
        float: left;
        margin-left: 30px;
    }
    .number2 {
        margin-left: 0px;
    }
    .number1 {
        margin-top: -120px;
    }
    .restaurant-class {
        margin-left: 30px;
    }
    .supermarket-class {
        margin-left: 30px;
    }
    /*.restaurant-box {
        transform: translateY(20px) translateX(-90px);
    }
    .restaurant-block {
        transform: translateX(60px);
    }
    .supermarket-block {
        transform: translateX(75px);
    }*/
    .trying-to {
        font-size: 45px;
        line-height: 50px;
        letter-spacing: -0.05em;
        text-align: left;
        width: 310px;
        margin-left: 0;
        transform: translateY(60px) translateX(30px);
    }
    .you-are-here {
        width: 320px;
        transform: translateY(40px) translateX(30px);
    }
    ul {
        margin-left: 30px;
        width: 380px;
        /*white-space: nowrap;*/
    }
    .list-text {
        margin-left: 0px;
        display: inline-block;
        width: 310px;
    }
    .list3 {
        width: 280px;
    }
    .list6 {
        width: 280px;
    }
    .check {
        display: inline-block;
    }
    p:nth-child(2) {
        transform: translateX(-15px);
    }
    button {
        margin-bottom: 90px;
    }
    .modal-row {
        width: 100%;
        height: 200%;
        background: rgba(0, 0, 0, 0.75);
        /*position: absolute;*/
        position: relative;
        top: 0;

        display: flex;
        justify-content: center;
        align-items: center;
    }

    .modal-content {
        position: relative;
        width: 350px;
        height: 570px;
        top: 0px;

        border-radius: 10px;
        padding: 5px;
        text-align: left;
        margin-left: 0px;
        margin-right: 0px;
        padding-top: 20px;
    }
    .modal-content h2 {
        margin-top: -10px;
        margin-right: 10px;
    }
    .modal-content h1 {
        font-size: 40px;
        line-height: 50px;
        /* or 117% */

        display: flex;
        align-items: center;
        letter-spacing: -0.05em;

        color: #464646;
        width: 320px;

        margin-top: 40px;
    }
    .modal-content input {
        width: 100%;
        height: 47px;
        border: none;
        border-bottom: 0.5px solid #000000;
        padding: 25px 0px 16px 0px;
        margin-bottom: 19px;


        font-size: 18px;
        line-height: 27px;
        letter-spacing: -0.05em;

        color: #464646;
    }
    .modal-content .email-input {
        margin-top: 20px;
    }
    .modal-content .submit-btn {
        padding: 0px;
        margin-top: 33px;
        height: 65px;
        border-radius: 10px;
        font-size: 26px;
    }

}



</style>
