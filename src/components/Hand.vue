<script setup>  
  import { reactive } from 'vue';
  import CardList from './CardList.vue'
  const Cards = reactive([
    {
      Id: 1,
      Name: 'one',
      Image: 'https://th.bing.com/th/id/OIP.GjyLaXhdKdaddDpIOMd0fAHaHa?pid=ImgDet&rs=1',
      Damage: 1
    },
    {
      Id: 2,
      Name: 'two',
      Image: 'https://th.bing.com/th/id/OIP.GjyLaXhdKdaddDpIOMd0fAHaHa?pid=ImgDet&rs=1',
      Damage: 2
    },
    {
      Id: 3,
      Name: 'three',
      Image: 'https://th.bing.com/th/id/OIP.GjyLaXhdKdaddDpIOMd0fAHaHa?pid=ImgDet&rs=1',
      Damage: 3
    },
    {
      Id: 4,
      Name: 'three',
      Image: 'https://th.bing.com/th/id/OIP.GjyLaXhdKdaddDpIOMd0fAHaHa?pid=ImgDet&rs=1',
      Damage: 3
    },
    {
      Id: 5,
      Name: 'two',
      Image: 'https://th.bing.com/th/id/OIP.GjyLaXhdKdaddDpIOMd0fAHaHa?pid=ImgDet&rs=1',
      Damage: 2
    },
  ]);
</script>

<template>
  <div class="Hand">
    <CardList Id="1" :Cards="Cards" />
  </div>
</template>

<style>
  .Hand {
    background-color: rgba(0,0,0,0.5);
    display: flex;
    justify-content: center;
  }
</style>