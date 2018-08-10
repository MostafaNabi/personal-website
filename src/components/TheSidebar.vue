<template>
  <div>
    <div id="container">
      <div id="background-color-wrapper">
        <div id="profile-wrapper">
          <div id="profile-picture-wrapper">
            <img id="profile-picture" v-bind:src="profilePicture"/>
          </div>
          <div id="profile-text-wrapper">
            <div id="profile-name"> Mostafa Nabi </div>
            <div id="profile-description"> Short about me here </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import profilePicture from '@/assets/profile_picture.jpg';

export default {
  name: 'TheRightPanel',
  data () {
    return {
      profilePicture: profilePicture
    };
  }
};
</script>

<style lang="scss" scoped>
  #container {
    position: static;
    display: flex;
    height: 100%;
    width: 300px;
  }

  #background-color-wrapper {
    width: 100%;
    height: 300px;
    background-color: #90CAF9;
  }

  #profile-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    width: 100%;
    margin-top: 30px;
  }

  #profile-picture {
    height: 180px;
    width: 180px;
  }

</style>
