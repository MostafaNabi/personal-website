<template>
  <div>
    <div id="container">
      <div id="profile-wrapper">
        <div id="profile-picture-wrapper">
          <router-link to="/" class="link">
            <img id="profile-picture" v-bind:src="profilePicture" alt="profile picture"/>
          </router-link>
        </div>
        <div id="profile-text-wrapper">
          <div id="profile-name"> Mostafa Nabi </div>
          <div id="profile-description"> Short about me here </div>
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
    width: 150px;
    background-color: #212121;
  }
  #profile-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    width: 100%;
    margin-top: 10px;
  }

  #profile-text-wrapper {
    color: white;
    text-align: center;
  }

  #profile-picture {
    height: 120px;
    width: 120px;
    border-radius: 50%;
  }

</style>
