<template>
  <div id="container">
    <the-sidebar id="sidebar"/>
    <div id="main">
      <the-navbar id="navbar"/>
      <router-view id="content"/>
    </div>
  </div>
</template>

<script>
import TheNavbar from '@/components/TheNavbar';
import TheSidebar from '@/components/TheSidebar';
export default {
  name: 'App',
  components: {
    TheNavbar,
    TheSidebar
  }
};
</script>

<style lang="scss">
  html, body {
    height: 100%;
    width: 100%;
    margin: 0px;
    padding: 0px;
    background-color: #dedede;
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
  }

  #content {
    padding-left: 10px;
  }
</style>
