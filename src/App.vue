<template>
  <div id="container">
    <div id="main">
      <the-navbar id="navbar"/>
      <div id="main-body">
        <router-view id="content"/>
        <the-profile-card id="profile"/>
      </div>
    </div>
  </div>
</template>

<script>
import TheNavbar from '@/components/TheNavbar';
import TheProfileCard from '@/components/TheProfileCard';
export default {
  name: 'App',
  components: {
    TheNavbar,
    TheProfileCard
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
    align-items: center;
  }

  #navbar {
    width: 100%;
  }

  #main-body {
    display: flex;
    justify-content: flex-end;
    height: 100%;
    width: 100%;
  }

  #content {
    max-width: 50%;
  }

  #profile {
    margin-top: 15px;
    margin-left: 5%;
    margin-right: 5%;
  }
</style>
