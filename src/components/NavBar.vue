<template>
  <nav class="navbar">
     <router-link to="/" class="back-button">
      <img class="logo-img"  src="../assets/logo.svg" alt="Vue logo" >
  </router-link>
  </nav>
</template>

<style>
.navbar {
display: flex;
width: 1920px;
height: 80px;
left: 0px;
top: 0px;
/* Background */
background: #050824;
}

/* Logo */
.logo-img {
position: absolute;
width: 171px;
height: 36px;
left: 405px;
top: 22px;
}


</style>
