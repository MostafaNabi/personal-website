<template>
  <div>
    <div id="content-menu-wrapper">
      <ul>
        <li> About Me </li>
        <li> Skills </li>
        <li> Work Experience
          <ul>
            <li> STFC </li>
            <li> ARM Holdings </li>
          </ul>
        </li>
      </ul>
    </div>
  </div>

</template>

<script>
export default {
  name: 'TheContentMenu'
};
</script>

<style lang="scss" scoped>
  #content-menu-wrapper {
    border: 1px solid lightgray;
    box-shadow: 3px 3px 5px 0 #ccc;
  }

</style>
