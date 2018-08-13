<template>
  <div>
    <div id="carousel-container">
      <div id="main-wrapper">
        <div id="left-arrow" class="carousel-arrow" v-on:click="decrementIndex()"></div>
        <img class="carousel-image"
            v-for="(image, i) in images" :key="image"
            v-bind:src="require('@/assets/'+image)"
            v-show="carouselIndex === i"
        />
        <div id="right-arrow" class="carousel-arrow" v-on:click="incrementIndex()"></div>
      </div>
      <div id="select-wrapper">
        <div class="select-button"
            v-for="(image, i) in images" :key="image"
            v-on:click="carouselIndex = i"
            v-bind:class="{'selected-button': carouselIndex === i}"
        >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Carousel',
  props: {
    // paths to images to load
    images: {
      type: Array,
      required: true
    }
  },

  data () {
    return {
      carouselIndex: 0
    };
  },

  methods: {
    incrementIndex () {
      if (this.carouselIndex < this.images.length - 1) {
        this.carouselIndex++;
      } else {
        this.carouselIndex = 0;
      }
    },

    decrementIndex () {
      if (this.carouselIndex > 0) {
        this.carouselIndex--;
      } else {
        this.carouselIndex = this.images.length - 1;
      }
    }
  }
};
</script>

<style lang="scss" scoped>
  #carousel-container {
    background-color: black;
  }

  #main-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 30px;
  }

  .carousel-image {
    width: 600px;
    height: 300px;
  }

  #left-arrow {
    width: 0;
    height: 0;
    border-bottom: 40px solid transparent;
    border-top: 40px solid transparent;
    border-right: 40px solid silver;
    margin-right: 10px;
  }

  #right-arrow {
    width: 0;
    height: 0;
    border-bottom: 40px solid transparent;
    border-top: 40px solid transparent;
    border-left: 40px solid silver;
    margin-left: 10px;
  }

  #left-arrow:hover {
    border-right-color: gray;
  }

  #right-arrow:hover {
    border-left-color: gray;
  }

  .carousel-arrow:hover {
    cursor: pointer;
  }

  #select-wrapper {
    display: flex;
    justify-content: center;
  }

  .select-button {
    height: 20px;
    width: 20px;
    border-radius: 50%;
    background-color: silver;
    margin: 10px;
  }

  .select-button:hover {
    cursor: pointer;
    background-color: gray;
  }

  .selected-button {
    background-color: gray;
  }
</style>
