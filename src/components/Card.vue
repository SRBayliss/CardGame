<script setup>
    const props = defineProps(['Id', 'Name', 'Image', 'Damage']);
</script>

<template>
    <div class="card" v-bind:id="Id">
        <div class="name">{{Name}}</div>
        <img class="image" v-bind:src="Image"/>
        <div class="damage">{{Damage}}</div>
    </div>
</template>

<style>
.card {
    width: 100px;
    height: 150px;
    margin: 5px;
    border: 1px solid white;
    background-color: grey;
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: large;
    opacity: 100%;
}

.name {
    text-align: center;
}

.image {
    width: 90px;
    height: 100px;
    display: block;
    margin-left: auto;
    margin-right: auto;
}

.damage {
    margin: 5px 5px 0 0;
    text-align: right;
}
</style>