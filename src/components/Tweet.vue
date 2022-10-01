<template>

    <div className="tweet">
      <!-- <img
        src="https://i.imgur.com/9yw1Fyw.jpg"
        className="profile"
        alt="profile"
      /> -->
      <ProfileImage/>
  
      <div className="body">
        <div className="top">
          <User/>
          <Timestamp/>
        </div>
        <Message message="Snoop doooooog"/>
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
  </script>
  <style scoped>
  a {
    color: #42b983;
  }
  </style>