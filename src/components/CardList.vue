<script setup>
    import Card from './Card.vue'
    const props = defineProps(['Id', 'Cards']);
</script>

<template>
    <div class="CardList">
        <Card v-for="Card in Cards" v-bind:Id="Card.Id" v-bind:Name="Card.Name" v-bind:Image="Card.Image" v-bind:Damage="Card.Damage"/>
    </div>
</template>

<style>
.CardList {
    display: flex;
    flex-direction: row;
}
</style>