<template>
  <div id="homepage-content">
    <div id="about-me" class="content-section">
      <div class="section-title-wrapper">
        <h1 class="section-title"> About Me </h1>
      </div>
      <div class="section-content-wrapper">

        <div class="section-content-visual">
          <img id="profile-picture" v-bind:src="profilePicture" alt="profile-picture"/>
        </div>

        <div class="section-content-text">
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
      </div>
    </div> <!-- close about me -->

    <div id="skills" class="content-section">
      <div class="section-title-wrapper">
        <h1 class="section-title"> Skills </h1>
      </div>
      <div class="section-content-wrapper">
        <div class="section-content-text">
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

        <div class="section-content-visual">
          <div class="logo-wrapper">
            <span class="tech-logo"> SPA </span>
            <span class="tech-logo"> Node.js </span>
            <span class="tech-logo"> Vuejs </span>
            <span class="tech-logo"> SASS </span>
            <span class="tech-logo"> Docker </span>
            <span class="tech-logo"> Progressive Web Apps </span>
          </div>
          <div class="logo-wrapper">
            <span class="tech-logo"> Docker </span>
            <span class="tech-logo"> Webpack </span>
            <span class="tech-logo"> Babel </span>
            <span class="tech-logo"> MySQL</span>
            <span class="tech-logo"> MongoDB </span>
            <span class="tech-logo"> Python </span>
            <span class="tech-logo"> Java </span>
            <span class="tech-logo"> C++ </span>
          </div>
        </div>

      </div>
    </div> <!-- close about me -->

  </div>
</template>

<script>
import profilePicture from '@/assets/profile_picture.jpg';
export default {
  name: 'TheHomePage',
  data () {
    return {
      profilePicture
    };
  }
};
</script>

<style lang="scss" scoped>

#home-page-content {
  width: 100%;
  height: 100%;
  background-color: white;
}

.content-section {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  height: 90%;
  width: 100%;
  background-color: #efedec;
  border-bottom: 1px solid black;
}

.content-section:nth-child(odd) {
  background-color: #efedec;
  color: #101112;
}

.content-section:nth-child(even) {
  background-color: #101112;
  color: #efedec;
}

.section-title-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 15px;
}

.section-title {
  margin: 0px;
  text-align: center;
  font-size: 56px;
  text-decoration: underline;
}

.section-content-wrapper {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  width: 100%;
}

.section-content-visual {
  display: flex;
  justify-content: center;
  min-width: 30%;

  #profile-picture {
    width: 240px;
    height: 240px;
  }
}
.section-content-text {
  font-size: 28px;
  max-width: 50%;
}

#skills {
  .section-content-visual {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #47a8b3;
    font-size: 24px;
    font-weight: bold;
  }

  .logo-wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin-bottom: 30px;
    max-width: 500px;
  }

  .tech-logo {
    padding: 5px;
    border-right: 1px solid #47a8b3;
  }

  .tech-logo:last-child {
    border-right: none;
  }
}
</style>
