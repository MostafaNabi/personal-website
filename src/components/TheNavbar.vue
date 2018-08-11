<template>
  <div>
    <div id="navbar-wrapper">
      <div id="cover-photo-wrapper">
      </div>
      <div id="navbar-menu-wrapper">
        <div id="navbar-links">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import coverPhoto from '@/assets/cover_photo.jpg';
export default {
  name: 'TheNavbar',
  data () {
    return {
      coverPhoto
    };
  }
};
</script>

<style lang="scss" scoped>
  #navbar-wrapper {
    width: 100%;
    background-color: white;
  }

  #cover-photo-wrapper {
    position: static;
    display: block;
    width: 100%;
    height: 200px;
    background-color: skyblue;
  }

  #navbar-wrapper {
    display: block;
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
