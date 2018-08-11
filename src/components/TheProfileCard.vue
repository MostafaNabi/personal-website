<template>
  <div>
    <div id="profile-wrapper">
      <div id="profile-picture-wrapper">
        <img id="profile-picture" v-bind:src="profilePicture" alt="profile-picture"/>
      </div>
      <div id="profile-text-wrapper">
        <ul>
          <li> Software Developer </li>
          <li> Email: mostafa_nabi@outlook.com </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import profilePicture from '@/assets/profile_picture.jpg';
export default {
  name: 'TheProfileCard',
  data () {
    return {
      profilePicture
    };
  }
};
</script>

<style lang="scss" scoped>
  #profile-wrapper {
    border: 1px solid lightgray;
    box-shadow: 3px 3px 5px 0 #ccc;
  }

  #profile-picture-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 5px;
  }

  #profile-picture {
    height: 120px;
    width: 120px;
    border-radius: 50%;
  }
</style>
