<template>
  <div class="photo-list">
    <div class="grid">
      <Photo
          class="grid__item"
          v-for="photo in photos"
          :key="photo.id"
          :item="photo"
      />
    </div>
  </div>
</template>