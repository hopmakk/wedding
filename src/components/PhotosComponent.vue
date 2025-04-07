<template>
    <div class="photo-gallery">
      <div 
        v-for="(photo, index) in photos" 
        :key="index" 
        class="photo-item">
        <img :src="getImageUrl(photo)" alt="Wedding photo" class="photo-image">
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'PhotoGallery',
    data() {
      return {
        photos: [
          'Title.png',
          'Texts.png',
          'April.png',
          'Hotel.png',
          'Clouds.png',
          'Pallet.png',
          'GuestList.png',
          'Footer.png',
        ]
      }
    },
    methods: {
      getImageUrl(photoName) {
        return require(`@/assets/${photoName}`);
      }
    }
  }
  </script>
  
  <style scoped>
  .photo-gallery {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  
  .photo-item {
    width: 100%;
    margin-bottom: 10px;
  }
  
  .photo-image {
    width: 100%;
    height: auto;
    display: block;
  }
  </style>