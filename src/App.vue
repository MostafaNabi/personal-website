<template>
  <div id="container">
    <div id="main">
      <the-navbar id="navbar"/>
      <div id="main-body">
        <router-view id="content"/>
      </div>
    </div>
  </div>
</template>

<script>
import TheNavbar from '@/components/TheNavbar';
import TheProfileCard from '@/components/TheProfileCard';
import TheContentMenu from '@/components/TheContentMenu';
export default {
  name: 'App',
  components: {
    TheNavbar,
    TheProfileCard,
    TheContentMenu
  }
};
</script>

<style lang="scss">
  html, body {
    height: 100%;
    width: 100%;
    margin: 0px;
    padding: 0px;
    color: #333;
  }
</style>

<style lang="scss" scoped>
  #container {
    display: flex;
    height: 100%;
    width: 100%;
  }

  #main {
    display: flex;
    height: 100%;
    width: 100%;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }

  #navbar {
    position: fixed;
    top: 0px;
    height: 50px;
    min-height: 50px;
    width: 100%;
    z-index: 1000;
  }

  #main-body {
    position: absolute;
    top: 50px;
    height: 100%;
    width: 100%;
  }

/*
  #menu {
    margin-top: 15px;
    margin-left: 5%;
    margin-right: 5%;
  }
*/
  #content {
    height: 100%;
    width: 100%;
  }

  /*

  #profile {
    margin-top: 15px;
    margin-left: 5%;
    margin-right: 5%;
  }
  */
</style>
