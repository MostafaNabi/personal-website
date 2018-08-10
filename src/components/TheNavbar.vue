<template>
  <div>
    <div id="navbar-wrapper">
      <div id="navbar-menu-wrapper">
        <div id="navbar-links">
          <span class="link"> Skills </span>
          <span class="link"> Work Experience </span>
          <span class="link"> Projects </span>
          <span class="link"> Education </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import profilePicture from '@/assets/profile_picture.jpg';
import DropdownMenu from '@/components/DropdownMenu';
export default {
  name: 'TheNavbar',
  components: {
    DropdownMenu
  }
};
</script>

<style lang="scss" scoped>
  #navbar-wrapper {
    width: 100%;
    background-color: white;
  }

  #title {
    margin-right: 20px;
  }

  #title-text {
    font-size: 26px;
    color: blue;
  }

  #profile-picture {
    margin-right: 20px;
  }

  #navbar-wrapper {
    display: flex;
    align-items: center;
  }

  #navbar-links {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding-left: 10px;

    span {
      margin-right: 10px;
      font-size: 24px;
    }
  }

  .link {
    text-decoration: none;
  }

  .link:hover {
    cursor: pointer !important;
    color: skyblue !important;
  }
</style>
