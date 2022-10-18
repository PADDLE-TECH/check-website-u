<template>
  <div class="register">
    <div class="color"></div>
    <!--<h1>This is an about page</h1>-->
    <appHeader></appHeader>

    <div class="container-fluid">
        <div class="grid-contain-1 row flex-column-reverse flex-md-row">
                <div class="first-container col-md-12">

                    <h3 class="we-are-obsessed slide-in">We are obsessed about making things work for you and your business!</h3>
                    <h3 class="how-we-built slide-in-delay">How we built the solution that works for you</h3>

                    <h3 class="our-expert">Our expert engineers use technically driven deep algorithm to power our QR code system which is the anchor of  our innovation.
                    The QR code technology is a faster way to send and receive data which eliminates every form of failure and disconnection in your transactions. </h3>
                </div>

                <!--<div class="col-md-6">
                    <div class="modal-content fade-up" id="form1">
                        <form action="https://formsubmit.co/checkretailer@gmail.com" method="POST">
                            <h1>Drop your details, we will surely reach back!</h1>
                            <input type="email" name="Email" placeholder="Email" class="email-input" required><br>
                            <input type="tel" name="Phone-number" placeholder="Phone number eg: 081*******3"  required><br>
                            <input type="text" name="Company-name" placeholder="Company name" required><br>
                            <input type="submit" value="Contact me!" class="submit-btn">
                        </form>
                    </div>
                </div>-->

        </div>
        <hr style="margin-left:10%;margin-right:10%">
        <form class="row form-submit" action="https://formsubmit.co/checkretailer@gmail.com" method="POST">
            <div class="nav">
                <div class="col-md-4 nav1"><h2 @click="backToStep1()" :class="step1 ? 'active' : 'not-active'">Branch Manager’s Information <h4 style="display:inline-block;font-size: 14px;"> (1of3)</h4></h2></div>
                <div class="col-md-4 nav2"><h2  @click="switchToStep2()" :class="step2 ? 'active' : 'not-active'">Company Information <h4 style="display:inline-block;font-size: 14px;"> (2of3)</h4></h2></div>
                <div class="col-md-4 nav3"><h2  @click="switchToStep3 ()" :class="step3 ? 'active' : 'not-active'">Branch Information <h4 style="display:inline-block;font-size: 14px;"> (3of3)</h4></h2></div>
                <div class="progress-path">
                    <div class="progress-bar" :style="step1 ? 'width:33%' : step2 ? 'width:66%' : 'width:100%' "></div>
                </div>
            </div>

            <div v-show="step1" class="step-1 step">
                <div class="row">
                    <div class="col-md-4">
                        <label>First Name</label><br>
                        <input type="text" placeholder="Enter manager’s first name" v-model="firstName">
                    </div>
                    <div class="col-md-4">
                        <label>Surname</label><br>
                        <input type="text" placeholder="Enter manager’s surname" v-model="lastName">
                    </div>
                    <div class="col-md-4">
                        <label>Gender</label><br>
                        <select v-model="gender" required>
                            <option value="" disabled selected>Click to select a gender</option>
                            <option value="male">Male</option>
                            <option value="female">Female</option>
                        </select>
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <label>E-mail Address</label><br>
                        <input type="email" placeholder="example@gmail.com" v-model="email">
                    </div>
                    <div class="col-md-4">
                        <label>Phone Number</label><br>
                        <input type="tel" placeholder="E.g 08130405070" v-model="phoneNumber">
                    </div>
                    <div class="col-md-4">
                        <label>Alternative Number (Optional)</label><br>
                        <input type="tel" placeholder="E.g 08130405070" v-model="alternativeNumber">
                    </div>
                </div>
                <div class="row nav-buttons">
                    <ul>
                        <li>Back</li>
                        <li style="background: #D40100;" @click="switchToStep2 ()">Continue</li>
                    </ul>
                </div>
            </div>

            <div v-show="step2" class="step-2 step">
                <div class="row">
                    <div class="col-md-4">
                        <label>Company Name</label><br>
                        <input type="text" placeholder="Enter company name" v-model="companyName">
                    </div>
                    <div class="col-md-4">
                        <label>Registered Name </label><br>
                        <input type="text" placeholder="Enter parent company name" v-model="registeredName">
                    </div>
                    <div class="col-md-4">
                        <label>CAC Number</label><br>
                        <input type="number" placeholder="E.g 1430035050" v-model="cacNumber">
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <label>Category</label><br>
                        <select v-model="category" required>
                            <option value="" disabled selected>Category</option>
                            <option value="Restaurant">Restaurant</option>
                            <option value="Supermarket">Supermarket</option>
                        </select>
                    </div>
                    <div class="col-md-4">
                        <label>Location</label><br>
                        <input type="text" placeholder="Enter location" v-model="location">
                    </div>
                    <div class="col-md-4">
                        <label>Address</label><br>
                        <input type="text" placeholder="Enter address" v-model="address">
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <label>Company E-mail Address</label><br>
                        <input type="email" placeholder="example@gmail.com" v-model="companyEmail">
                    </div>
                    <div class="col-md-4">
                        <label>Phone Number</label><br>
                        <input type="tel" placeholder="E.g 08130405070" v-model="companyPhone">
                    </div>
                    <div class="col-md-4">
                        <label>Alternative Number (Optional)</label><br>
                        <input type="tel" placeholder="E.g 08130405070" v-model="companyAlternativePhone">
                    </div>
                </div>
                <div class="row nav-buttons">
                    <ul>
                        <li style="background: #F87D5E;" @click="backToStep1()">Back</li>
                        <li style="background: #D40100;" @click="switchToStep3 ()">Continue</li>
                    </ul>
                </div>
            </div>

            <div v-show="step3" class="step-1 step">
                <input name="First_Name" :value="firstName" style="display: none">
                <input name="Last_Name" :value="lastName" style="display: none">
                <input name="Gender" :value="gender" style="display: none">
                <input name="Email Address" :value="email" style="display: none">
                <input name="Phone_number" :value="phoneNumber" style="display: none">
                <input name="Alternative_number" :value="alternativeNumber" style="display: none">
                <input name="Company_Name" :value="companyName" style="display: none">
                <input name="Registered_Name" :value="registeredName" style="display: none">
                <input name="CAC_Number" :value="cacNumber" style="display: none">
                <input name="Category" :value="category" style="display: none">
                <input name="Location" :value="location" style="display: none">
                <input name="Address" :value="address" style="display: none">
                <input name="Company_Email" :value="companyEmail" style="display: none">
                <input name="Company_phone_NUmber" :value="companyPhone" style="display: none">
                <input name="Company_alternative_phone" :value="companyAlternativePhone" style="display: none">
                <div class="row">
                    <div class="col-md-4">
                        <label>Number of Tables</label><br>
                        <input type="number" name="Number_of_tables" placeholder="1020" >
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <label>Bank Name</label><br>
                        <input type="text" name="Bank_name" placeholder="Enter bank name" >
                    </div>
                    <div class="col-md-4">
                        <label>Account Name</label><br>
                        <input type="text" name="Account_name" placeholder="Enter account name" >
                    </div>
                    <div class="col-md-4">
                        <label>Account Number</label><br>
                        <input type="number" name="Account_number" placeholder="E.g 0582501930">
                    </div>
                </div>
                <div class="row nav-buttons">
                    <ul>
                        <li style="background: #F87D5E;" @click="backToStep2()">Back</li>
                        <input type="submit" value="submit">
                        <!--<li style="background: #D40100;">Submit</li>-->
                    </ul>
                </div>
            </div>

        </form>



        <div class="row row2register">

            <aos-vue animation="" class="col-md-6 col-sm-12">
                <aos-vue animation="fade-right">
                    <img src="../assets/images/Vector-34-ii.webp" class="table">
                </aos-vue>
                <img src="../assets/images/Vector-34-ii.webp" class="table2">

            </aos-vue>



            <aos-vue animation="fade-left" class="col-md-6 col-sm-12">
                <div class="number1">
                    <img src="../assets/pic1/pic2/01.png" class="num1"><br>
                    <p class="restaurant-class">Restaurant</p>
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


        <div class="row row2register">
            <!--<>-->
                <aos-vue animation="fade-right" class="col-md-6">
                <div class="number2">
                    <img src="../assets/pic1/pic2/02.png" class="num1"><br>
                    <p class="supermarket-class">Supermarket</p>

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
                    <img src="../assets/images/Vector-33-ii.webp" class="woman-with-phone-pic">
                </aos-vue>
            </aos-vue>
        </div>





        <oneApp></oneApp>
        <trustedBy></trustedBy>
        <footerLinks></footerLinks>
        </div>
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
        form2: false,
        step1: true,
        step2: false,
        step3: false,

        firstName: "",
        lastName: "",
        gender: "",
        email: "",
        phoneNumber: "",
        alternativeNumber: "",
        companyName: "",
        registeredName: "",
        cacNumber: "",
        category: "",
        location: "",
        address: "",
        companyEmail: "",
        companyPhone: "",
        companyAlternativePhone: ""
    }
  },
  methods: {
    switchToStep2 () {
        this.step2 = true,
        this.step1 = false,
        this.step3 = false
        //this.step2 = true
        //this.step3 = false
    },
    switchToStep3 () {
        this.step1 = false,
        this.step2 = false,
        this.step3 = true
    },
    backToStep1() {
        this.step3 = false
        this.step2 = false,
        this.step1 = true
    },
    backToStep2() {
        this.step2 = true,
        this.step3 = false
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
    /*height: 800px;*/
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
    /*width: 550px;*/
    width: 850px;
    margin: auto;

    margin-top: 182px;
    position: relative;
    /*left: 50%;
    transform: translateX(-44%);*/
    color: black;
    font-family: 'Euclid Circular A';

    /* margin-left: 131px; */
    /*text-align: left;*/
}
.how-we-built {
    /*font-family: 'poppins';
    text-align: center;
    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 30px;
    text-align: left;
    margin-top: 91px;
    color: black;*/

    /*margin-left: 90px;*/
    font-family: 'poppins';
    /*text-align: center;*/
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 25px;
    /*text-align: left;*/
    /*width: 561px;*/
    position: relative;
    /*left: 50%;
    transform: translateX(-44%);*/
    margin: 0 auto;
    margin-top: 91px;
    color: black;
}
.our-expert {
    font-family: 'poppins';
    /*text-align: center;*/
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    width: 561px;
    position: relative;
    margin: auto;
    /*left: 50%;
    transform: translateX(-44%);*/
    margin-top: 26px;
    color: black;
}
.progress-path {
    position: relative;
    height: 7px;
    width: 100%;
    background: #BABABA;
    border-radius: 4px;
    margin-top: 5px;
}
.progress-bar {
    position: absolute;
    height: 7px;
    background: #D40100;
    border-radius: 4px;
    /*width: 33%;*/
}
.form-submit {
    margin-bottom: 50px;
    /*border: 4px solid green;*/
    padding: 8%;
}
.form-submit .nav h2 {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    line-height: 125%;
    text-align: left;
    display: inline-block;
    cursor: pointer;
}
.active {
    color: #000000;
}
.not-active {
    color: #BABABA;
}
.form-submit .nav {
    margin-bottom: 63px;
}
.form-submit .col-md-4 {
    padding-right: 35px;
    /*border: 2px solid orange;*/
}

.form-submit .step {
    text-align: left;
}
.step label {
    font-weight: 600;
    font-size: 14px;
    line-height: 16px;
    margin-bottom: 4px;
}
.step input, .step select {
    border: 1px solid #CBD2E0;
    border-radius: 6px;
    width: 331px;
    height: 44px;
    padding-left: 10px;
    margin-bottom: 15px;
}
input[type='submit'] {
    width: 230px;
    /*padding-top: 15.2px;
    padding-bottom: 15.2px;*/
    display: inline-block;
    background: #D40100;
    color: #fff;
    height: 58px;
}
.nav-buttons ul{
    /*display: flex;
    justify-content: space-between;*/
    text-align: right;
    /*border: 2px solid yellow;*/
    margin-left: -3%;
    margin-top: 48px;

}
.nav-buttons li {
    display: inline-block;
    list-style: none;
    text-align: center;
    background: #BABABA;
    width: 230px;
    /*height: 44px;*/
    padding-top: 15.2px;
    padding-bottom: 15.2px;
    border-radius: 4px;
    color: #fff;
    cursor: pointer;
}
.nav-buttons li:nth-child(1) {
    margin-right: 20px;
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
        /*height: 1200px;*/
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
        /*margin-top: 30px;*/

        left: 0%;
        transform: translateX(0%);
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
    .form-submit .col-md-4 {
        padding-right: 0px;
        /*border: 2px solid orange;*/
    }
    .step input, .step select {
        width: 100%;
    }
    .nav-buttons ul{
        text-align: left;
        /*border: 2px solid yellow;*/
        margin-left: -3%;
        margin-top: 48px;

    }
    input[type='submit'] {
        width: 130px;
    }
    .nav-buttons li {
        display: inline-block;
        list-style: none;
        text-align: center;
        background: #BABABA;
        width: 130px;
        /*height: 44px;*/
        padding-top: 15.2px;
        padding-bottom: 15.2px;
        border-radius: 4px;
        color: #fff;
        cursor: pointer;
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
        /*margin-top: -500px;*/
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
        margin-top: -100px;
    }
    .restaurant-class {
        margin-left: 30px;
    }
    .supermarket-class {
        margin-left: 30px;
    }

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
