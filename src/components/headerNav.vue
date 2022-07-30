<template>
    <div id="nav-background">
        <nav class="navbar navbar-expand-lg bg-white py-3">
  <div class="container-fluid">
    <a class="navbar-brand" href="#"><img src="../assets/images/logo.png"></a>
    <div @click="showMenu = !showMenu" class="navbar-toggler " type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"><img v-show="!showMenu" src="../assets/icons/menu-bar.png" class="menu-bar"> <img v-show="showMenu" src="../assets/icons/close-icon.svg" class="menu-bar"> </span>
    </div>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <router-link to="/" exact > Home</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/how-it-works" exact > I &nbsp<img src="../assets/images2/love-2.png" class="heart"> &nbsp &nbsp my customer</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/about" exact >About us</router-link>
        </li>
        <li class="nav-item dropdown">
          <router-link to="/register" exact>Register as a Merchant</router-link>

        </li>
        <!--<li class="nav-item">
          <router-link to="/policy" exact>Privacy Policy</router-link>
        </li>-->
      </ul>
      <form class="d-flex" role="search">
        <button class="download-button" ><a href="https://play.google.com/store/apps/details?id=com.paddletech.check">Download App </a><img src="../assets/images/Vector-2.png"></button>
      </form>
    </div>
  </div>
</nav>
    </div>
</template>

<script>

export default {
  name: 'AboutView',
  data() {
    return {
        showMenu: false
    }
  }
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@500&family=Poppins:wght@300;500;600&display=swap');
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');
* {
    margin: 0%;
    padding: 0%;
    font-family: 'Euclid Circular A';
}

@keyframes bounce {
    from {transform: translateY(-10px);};
    to {transform: translateY(0px);}
}

ul {
    transform: translateX(60px);
}
nav {
    /*margin: 15px;*/
    transform: translateY(15px);
    margin-left: 81px;
    margin-right: 81px;
    border-radius: 50px;
}
.navbar {
    /*border: 1px solid red;*/
    padding: 60px 30px 60px 30px;
}
nav img {
    height: 50px;
    width: 150px;
}
li {
    font-size: 16px;
    line-height: 22px;
    margin-left: 20px;
    margin-right: 20px;
    font-family: Inter;
    font-weight: 400;
    padding-top: 10px;


}
li:hover {
    transform: translateY(-5px);
    transition: all 0.4s ease;
}
li:nth-child(1) {
    animation-name: bounce;
    animation-duration: 1.5s;
    transition: all 0.4s ease;
}
li:nth-child(2) {
    animation-name: bounce;
    animation-duration: 1.5s;
    animation-delay: 0.5s;
    transition: all 0.4s ease;
    position: relative;
}
li:nth-child(3) {
    animation-name: bounce;
    animation-duration: 1.5s;
    animation-delay: 1s;
    transition: all 0.4s ease;
}
li:nth-child(4) {
    animation-name: bounce;
    animation-duration: 1.5s;
    animation-delay: 1.5s;
    transition: all 0.7s ease-in-out;
}

.heart {
    transform: scale(1.5) translateY(5px);
    /*height: 100%;
    width: 100%;*/
    width: 10px;
    height: 10px;
    /*display: inline-block;*/
    position: absolute;

}
a {
    color: black;
    text-decoration: none;
    font-size: 18px;
    line-height: 22px;
}
a:hover {
    color: #D392C5;

}
.download-button {
    padding: 14px 36px 16px 29px;
    /*width: 230px;
    height: 62px;*/
    border-radius: 40px;
    font-family: 'Inter';
    font-style: normal;
    color: #fff;
    background-color: black;
    padding-left: -2px;
    text-align: center;
    transform: scale(0.95);
}
.download-button a {
    color: #fff;
}
button img {
    width: 32px;
    height: 20px;
    padding: 2px;
    transform: translateX(20px);
}
.navbar-toggler  {
    /*color: rgb(255, 255, 255);*/
    margin-right: -20px;
}
/*.navbar-toggler span {
    color: rgb(2, 0, 0);
    width: 22px;
    height: 2px;
}*/
#nav-background {
    /*background: #a728a7;*/
    margin: 0%;
    padding: 0%;
    top: 0%;

}
.menu-bar {
    width: 100%;
    height: 100%;
    transform: 0.4s;
}
.router-link {
    text-decoration: none;

}

.router-link-active {
  /*background: #fff;*/
  /*color: #b92828;*/
  color: black;
  padding: 5px;
  /*border-radius: 5px;*/

  border-bottom: 3px solid #730319;
;
}


@media screen and (max-width: 700px){
    ul {
        text-align: left;
        transform: translateX(0px);
    }
    nav {
        margin: 0;
        transform: translateY(0px);
        border-radius: 0%;
    }
    nav img {
        height: 40px;
        width: 130px;
    }
    li {
        margin-left: 0%;
        margin-right: 0%;
        margin-top: 15px;
    }

    button img {
        width: 32px;
        height: 20px;
    }
    .download-button {
        margin: 10px 0px 10px 0px;
    }
}
</style>