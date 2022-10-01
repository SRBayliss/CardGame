<script setup>
  import { ref } from 'vue';
  import Hand from './Hand.vue';
  const props = defineProps(['Side']);
  const height = ref(window.innerHeight / 2);
</script>

<template>
  <div v-bind:class="props.Side" class="Zone">
    <PlayArea />
    <Bin />
    <Hand />
    <Deck />
  </div>
</template>

<style>
.Zone {
  height: 484px/* v-bind(height); */

}
  
.Player {  
  background-color: cyan;
}
.Player > .Hand {
  width: 100%;
  position: fixed;
  bottom: 0;
}

.Opponent {
  background-color: red;
}

</style>