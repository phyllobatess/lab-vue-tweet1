<template>

    <div className="tweet">
      <!-- <img
        src="https://i.imgur.com/9yw1Fyw.jpg"
        className="profile"
        alt="profile"
      /> -->
      <ProfileImage 
      :image="imageFather" 
      :imageAlt="'${userFather.name}- Profile Image'"/>
   
      <div className="body">
        <div className="top">
          <User :user="userFather"/>
          <Timestamp v-bind:timestamp="timestampFather"/>
        </div>
        <Message v-bind:message="messageFather"/>
        <Actions/>
     
      </div>
  
      <i class="fas fa-ellipsis-h"></i>
    </div>
  </template> 

  
  <script setup>
    import Actions from "./Actions.vue";
    import Message from "./Message.vue";
    import Timestamp from "./Timestamp.vue";
    import User from "./User.vue";
    import ProfileImage from "./ProfileImage.vue";
import { stringify } from "postcss";


defineProps({
  messageFather:{
    type:String,
  },
  timestampFather: {
    type:String,
  },
  userFather:{
    type: Object,
  },
  imageFather: {
    type:String,
  },
  imageAlt:{
    type: String,
  },
});


  </script>
  <style scoped>
  a {
    color: #42b983;
  }
  </style>