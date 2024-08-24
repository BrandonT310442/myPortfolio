<script setup>
import { ref, onMounted } from 'vue';

const textLines = ref([
  "Hello! 👋",
  "I'm <b>Brandon</b>, an innovative fullstack developer",
  "studying Computer Science at",
  "the University of Toronto."
]);

const displayText = ref(textLines.value.map(() => ''));
const typingSpeed = 15;

const typeText = (lineIndex) => {
  if (lineIndex >= textLines.value.length) return;

  const fullText = textLines.value[lineIndex];
  let charIndex = 0;

  const interval = setInterval(() => {
    if (charIndex < fullText.length) {
      displayText.value[lineIndex] += fullText[charIndex];
      charIndex++;
    } else {
      clearInterval(interval);
      setTimeout(() => typeText(lineIndex + 1), 500);
    }
  }, typingSpeed);
};

onMounted(() => {
  typeText(0);
});
</script>

<template>
  <div class="intro">
    <div class="media">
      <div class="media-content" id="wrap-text">
        <p class="is-size-3" v-html="displayText[0]"></p>
        <p class="is-size-3" v-html="displayText[1]"></p>
        <p class="is-size-3" v-html="displayText[2]"></p>
        <p class="is-size-3" v-html="displayText[3]"></p>
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
