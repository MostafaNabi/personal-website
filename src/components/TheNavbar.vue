<template>
  <div>
    <div id="navbar-wrapper">
      <div id="navbar-menu-wrapper">
        <div id="navbar-links">
          <span class="link"> About Me </span>
          <span class="link"> Skills </span>
          <span class="link"> Work Experience </span>
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
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    height: 100%;
    width: 100%;
    background-color: #587b7f;
  }

  #navbar-links {
    display: flex;
    justify-content: center;;
    align-items: center;
    margin-bottom: 10px;

    .link {
      font-size: 24px;
      text-decoration: underline;
      color: white;
      padding-left: 15px;
      padding-right: 15px;
      border-right: 1px solid white;
    }

    .link:last-child {
      border-right: none;
      padding-right: none;
    }

    .link:hover {
      cursor: pointer !important;
      color: #4eb8c4 !important;
    }
  }

</style>
