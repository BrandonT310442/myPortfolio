<script setup>
</script>

<template>
  <div class="intro">
    <div id="content" class="media">
      <div class="media-content" id="wrap-text">
        <p class="is-size-3">Hello! 👋</p>
        <br>
        <p class="is-size-3">
          I'm <strong>Brandon</strong>, an innovative fullstack developer
          <br />
          studying Computer Science at
          <br>
          the University of Toronto.
        </p>

      </div>

      <div class="media-right">
        <img id="emoji" src="../assets/memoji.png.jpeg" />
      </div>
    </div>
  </div>
</template>



<style scoped>
.intro {
  height: 105vh;
  margin-top: 100px;
  /* Any other styles you need */
}

#wrap-text {
  margin-top: 100px;
  margin-right: 50px;
  z-index: 1.0;
  transform: translateX(10%);
}

#emoji {
  width: 375px;
  height: 375px;
  transform: scaleX(-1) rotate(40deg);
  position: absolute;
  right: -105px;
  z-index: 1;

}
</style>