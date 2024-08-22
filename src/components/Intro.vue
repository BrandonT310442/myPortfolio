<template lang="">
    <div id="content" class="media">
      <div class="media-content" id="wrap-text">
        <p class="is-size-3">Hello 👋!</p>
        <br>
        <p class="is-size-3">
          I'm <strong>Brandon</strong>, a fullstack developer
          <br />
          studying Computer Science at
          the University of Toronto.
        </p>
      </div>
  
      <div class="media-right">
        <img id="emoji" src="../assets/aremoji.png" />
      </div>
    </div>
  </template>
  
  <script>
  export default {};
  </script>
  
  <style scoped>
  #wrap-text {
    margin-top: 100px;
    margin-left: 50px;
    margin-right: 50px;
    z-index: 1.0;
  }
  
  #emoji {
    width: 375px;
    height: 375px;
    transform: rotate(-40deg); 
    position: absolute;
  right: -115px; /* Move the image beyond the right edge of the screen */
  z-index: -1;

  }
  </style>
  