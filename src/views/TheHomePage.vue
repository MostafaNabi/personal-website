<template>
  <div id="homepage-content">

    <div id="about-me" class="content-section">
      <div class="section-title-wrapper">
        <h2 class="section-title"> About Me </h2>
        <i class="material-icons">arrow_right</i>
      </div>
      <div class="section-content-wrapper">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Sapien faucibus et molestie ac feugiat.
          Nulla pharetra diam sit amet nisl. Integer quis auctor elit sed. Dignissim suspendisse in est ante in nibh mauris cursus mattis. Eu lobortis elementum nibh tellus molestie nunc.
          Sed faucibus turpis in eu mi. Quis imperdiet massa tincidunt nunc pulvinar sapien et.
          Netus et malesuada fames ac turpis egestas maecenas pharetra. Sagittis purus sit amet volutpat consequat mauris nunc.
          Varius quam quisque id diam vel quam elementum. Ullamcorper eget nulla facilisi etiam dignissim.
          Est ullamcorper eget nulla facilisi etiam. Gravida dictum fusce ut placerat orci nulla pellentesque.
          Viverra vitae congue eu consequat ac felis.
        </p>
      </div>
    </div> <!-- close about me -->

    <div id="skills" class="content-section">
      <div class="section-title-wrapper">
        <h2 class="section-title"> Skills </h2>
        <i class="material-icons">arrow_right</i>
      </div>
      <div class="section-content-wrapper">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Sapien faucibus et molestie ac feugiat.
          Nulla pharetra diam sit amet nisl. Integer quis auctor elit sed. Dignissim suspendisse in est ante in nibh mauris cursus mattis. Eu lobortis elementum nibh tellus molestie nunc.
          Sed faucibus turpis in eu mi. Quis imperdiet massa tincidunt nunc pulvinar sapien et.
          Netus et malesuada fames ac turpis egestas maecenas pharetra. Sagittis purus sit amet volutpat consequat mauris nunc.
          Varius quam quisque id diam vel quam elementum. Ullamcorper eget nulla facilisi etiam dignissim.
          Est ullamcorper eget nulla facilisi etiam. Gravida dictum fusce ut placerat orci nulla pellentesque.
          Viverra vitae congue eu consequat ac felis.
        </p>
      </div>
    </div> <!-- close skills -->

    <div id="skills" class="content-section">
      <div class="section-title-wrapper">
        <h2 class="section-title"> Work Experience </h2>
        <i class="material-icons">arrow_right</i>
      </div>

      <div class="section-subtitle-wrapper">
        <h3 class="section-subtitle"> STFC </h3>
      </div>
      <div class="section-content-wrapper">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Sapien faucibus et molestie ac feugiat.
          Nulla pharetra diam sit amet nisl. Integer quis auctor elit sed. Dignissim suspendisse in est ante in nibh mauris cursus mattis. Eu lobortis elementum nibh tellus molestie nunc.
          Sed faucibus turpis in eu mi. Quis imperdiet massa tincidunt nunc pulvinar sapien et.
          Netus et malesuada fames ac turpis egestas maecenas pharetra. Sagittis purus sit amet volutpat consequat mauris nunc.
          Varius quam quisque id diam vel quam elementum. Ullamcorper eget nulla facilisi etiam dignissim.
          Est ullamcorper eget nulla facilisi etiam. Gravida dictum fusce ut placerat orci nulla pellentesque.
          Viverra vitae congue eu consequat ac felis.
        </p>
      </div> <!-- close stfc -->

      <div class="section-subtitle-wrapper">
        <h3 class="section-subtitle"> ARM Holdings </h3>
      </div>
      <div class="section-content-wrapper">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Sapien faucibus et molestie ac feugiat.
          Nulla pharetra diam sit amet nisl. Integer quis auctor elit sed. Dignissim suspendisse in est ante in nibh mauris cursus mattis. Eu lobortis elementum nibh tellus molestie nunc.
          Sed faucibus turpis in eu mi. Quis imperdiet massa tincidunt nunc pulvinar sapien et.
          Netus et malesuada fames ac turpis egestas maecenas pharetra. Sagittis purus sit amet volutpat consequat mauris nunc.
          Varius quam quisque id diam vel quam elementum. Ullamcorper eget nulla facilisi etiam dignissim.
          Est ullamcorper eget nulla facilisi etiam. Gravida dictum fusce ut placerat orci nulla pellentesque.
          Viverra vitae congue eu consequat ac felis.
        </p>
      </div> <!-- close stfc -->
    </div> <!-- close work experience -->
  </div>
</template>

<script>
export default {
  name: 'TheHomePage'
};
</script>

<style lang="scss" scoped>

#home-page-content {
  background-color: white;
}

.section-title-wrapper {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  border-bottom: 1px solid black;
  margin-top: 15px;
  margin-bottom: 15px;
}

.section-title {
  margin: 0px;
}

.section-subtitle-wrapper {
  display: flex;
  justify-content: flex-start;
  align-items: center;

  .section-subtitle {
    color: gray;
    margin-right: 10px;
  }

  .section-subtitle:hover {
    color: skyblue;
    cursor: pointer;

    ::after {
      content: "<i class='material-icons'>open_in_new</i>";
    }
  }
}
</style>
