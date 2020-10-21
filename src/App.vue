<template>
  <div id="app" class="big-container">
    <v-header></v-header>
    <v-emoji></v-emoji>
    <v-piano></v-piano>
    <v-note></v-note>
  </div>
</template>

<script>
// import func from '../vue-temp/vue-editor-bridge';
import VHeader from '@/components/VHeader'
import VEmoji from '@/components/VEmoji'
import VPiano from  '@/components/VPiano'
import VNote from  '@/components/VNote'
export default {
  name: "App",
  components: {
    VHeader,
    VEmoji,
    VPiano,
    VNote
  },
};

</script>

<style lang="postcss" scoped>
.big-container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: linear-gradient(135deg, #ff9d6c 0%, #bb4e75 100%);
}

@media (max-width: 700px) {
  .big-container {
    justify-content: space-around;
  }
  .container-piano,
  .container-emoji,
  .container-title {
    margin: 0;
  }
}
</style>