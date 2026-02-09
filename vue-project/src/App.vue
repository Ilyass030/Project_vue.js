<template>
  <div>
    <h1>Dog Center</h1>
    <div id="dog-gallery">
      <DogCard
        v-for="dog in dogsData"
        :key="dog.id"
        :name="dog.name"
        :age="dog.age"
        :breed="dog.breed"
        :pictureUrl="dog.pictureUrl"
        :soundUrl="dog.soundUrl"
      />
    </div>
  </div>
</template>

<script setup>
import dogsData from './dogsData'     
import DogCard from './components/DogCard.vue'
import DogCard from './components/NewsSlider.vue'
</script>