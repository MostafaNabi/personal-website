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
            Hello! I am a software developer living in Oxfordshire, I am currently working at Science and Technology Facilities Council (STFC) as graduate developer.
            The role is very varied with work ranging from web development to system administration, I am currently looking to specialise in modern Web Development
            and want to move back to my home town in Birmingham.
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

          </p>
        </div>

        <div class="section-content-visual">
          <div class="logo-wrapper">
            <span class="tech-logo"> SPA </span>
            <span class="tech-logo"> Node.js </span>
            <span class="tech-logo"> Vuejs </span>
            <span class="tech-logo"> SASS </span>
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
    </div> <!-- close skills -->

    <div id="stfc" class="content-section">
      <div class="section-title-wrapper">
        <h1 class="section-title"> Science and Technology Facilities Council </h1>
      </div>
      <div class="section-content-wrapper">
        <div class="section-content-visual">
          <carousel v-bind:images="['cover_photo.jpg', 'dafni-website-1.png', 'profile_picture.jpg']" />
        </div>
        <div class="section-content-text">
          <p>
            As part of the graduate training scheme we work on different projects every 6months to build broader knowledge.
            My most notable project was DAFNI (Data Analytics for National Infrastructure).
            The goal of DAFNI is to host all manners of data relating to infrastructure to allow researchers easy access to
            datasets and to run their models on our HPC infrastructure. DAFNI is still in the early stages of its lifecycle,
            my role within the project was to begin development on the DAFNI web platform, starting with data-catalogue,
            an online catalogue displaying metadata on all datasets hosted by DAFNI.
          </p>
          <p>
            Although joining the project as a graduate trainee, I was given a great deal of responsibility and freedom in developing the front-end.
            For the majority of my 6months on this project I was the sole front-end developer and was given the freedom to choose the technology stack
            and draw up the designs. I used Vue.js as my development framework (a framework similar to Angular) with SASS
            for the styling and async/await and Promises for doing AJAX calls. I am using the Mocha, Chai and Sinon stack writing unit tests.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import profilePicture from '@/assets/profile_picture.jpg';
import carousel from '@/components/Carousel';
export default {
  name: 'TheHomePage',
  components: {
    carousel
  },

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
  min-height: 90%;
  background-color: #efedec;
  border-bottom: 1px solid black;
  padding: 0 10%;
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
  font-size: 36px;
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
  font-size: 1.5rem;
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
    padding-right: 10px;
    padding-left: 10px;
    border-right: 1px solid #47a8b3;
  }

  .tech-logo:last-child {
    border-right: none;
  }
}
</style>
