<template>
  <nav>
    <router-view v-slot="{ Component }">
      <transition name="route" mode="out-in" appear>
        <component :is="Component"></component>
      </transition>
    </router-view>
    <!--<router-view/>-->
    <!--<router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>-->
  </nav>

</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
* {
    margin: 0%;
    padding: 0%;
}
/*nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}*/

nav a.router-link-exact-active {
  color: #ffffff;
}


.route-enter-from {
  opacity: 0;
  transform: translateX(1800px);
  /*transform: scaleX(0);*/
}
.route-enter-to {
  opacity: 1;
  transform: translateX(0);
  /*transform: scaleX(1);*/
}
.route-enter-active {
  transition: all 0.4s ease;
}

.route-leave-from {
  opacity: 1;
  transform: translateX(0);
   /*transform: scaleX(1);*/
}
.route-leave-to {
  opacity: 0;
  transform: translateX(-1800px);
  /*transform:scaleX(0);*/
}
.route-leave-active {
  transition: all 0.4s ease;

}


.slide-in {
    animation-name: slide-in;
    animation-duration: 1.5s;
}
.slide-in-delay1 {
    animation-name: slide-in;
    animation-duration: 2.5s;
    /*animation-delay: 0.5s;*/
}

.slide-out {
    animation-name: slide-out;
    animation-duration: 1.5s;
}

</style>
