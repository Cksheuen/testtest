<script>
export default {
  data() {
    return {
      photos: [
        { id: 1, url: '/cuc.jpg' },
        { id: 2, url: '/cuc.jpg' },
        { id: 3, url: '/cuc.jpg' },
        { id: 4, url: '/cuc.jpg' },
        { id: 5, url: '/cuc.jpg' },
        { id: 6, url: '/cuc.jpg' },
        // Add more photos here
      ],
    }
  },
}
</script>

<template>
  <div class="photo-wall">
    <div v-for="photo in photos" :key="photo.id" class="photo">
      <img :src="photo.url" alt="photo">
    </div>
  </div>
</template>

<style>
.photo-wall {
  display: flex;
  flex-wrap: wrap;
}

.photo {
  flex: 0 0 33.33%;
  padding: 10px;
}

.photo img {
  width: 100%;
  height: auto;
}
</style>
