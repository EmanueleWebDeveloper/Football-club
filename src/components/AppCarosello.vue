<template>
     <div class="carousel">
    <div class="carousel-container">
      <button class="arrow left" @click="prevSlide">&#10094;</button>
      <div class="slides">
        <div v-for="(slide, index) in slides" :key="index" :class="{ active: index === currentIndex }">
          <!-- Contenuto del singolo slide -->
          <img :src="slide.image" :alt="slide.alt">
        </div>
      </div>
      <button class="arrow right" @click="nextSlide">&#10095;</button>
    </div>
  </div>
</template>
  
  <script>
  
  import { store } from '../store'

  
  export default {
    name: 'AppCarosello',
    data() {
        return {
      slides: [
        { image: '', alt: 'Description 1' },
        { image: '', alt: 'Description 2' },
        { image: '', alt: 'Description 3' },
        
      ],
      currentIndex: 0
    };
  },
  methods: {
    prevSlide() {
      this.currentIndex = (this.currentIndex - 1 + this.slides.length) % this.slides.length;
    },
    nextSlide() {
      this.currentIndex = (this.currentIndex + 1) % this.slides.length;
    }
  }
};
</script>
  
  <style lang="scss" scoped>
.carousel {
  width: 100%;
  margin: auto;
}

.carousel-container {
  position: relative;
}

.slides {
  display: flex;
  overflow: hidden;
}

.slides div {
  flex: 0 0 100%;
  transition: transform 0.5s ease;
}

.arrow {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(255, 255, 255, 0.5);
  border: none;
  color: black;
  font-size: 2em;
  cursor: pointer;
  padding: 10px;
  z-index: 1;
}

.arrow.left {
  left: 0;
}

.arrow.right {
  right: 0;
}

.arrow:hover {
  background: rgba(255, 255, 255, 0.8);
}

.active {
  display: block;
}
  </style>
  
