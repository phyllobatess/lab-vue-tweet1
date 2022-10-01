<template>
  <img
    v-bind:src="image"
    className="profile"
    alt="profile"
  />
</template>
 
 
 
 <script setup>
  defineProps({
    image:{
      type: String,
      default:"https://www.binaural.es/wp-content/uploads/2011/02/moby.jpg"
    },
    imageAlt: {
      type: String,
      default: "Moby!"
    },
  });
 </script>


 