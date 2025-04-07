<template>
  <div>
    <PhotosComponent/>
  </div>
</template>

<script>
import PhotosComponent from "./components/PhotosComponent.vue";

export default {
  name: 'App',
  components: {
    // HeaderSection, MainSection, FirstText, Calendar, FooterSection
    PhotosComponent
  }
}
</script>
