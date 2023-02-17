<template>
  <div class="col-3 memes">Meme</div>
  <p>{{ meme.name }}</p>
  <img :src="meme.url" :alt="name" class="fluid" />
</template>

<script>


export default {
  props: {
    meme: Object,
  }
}
</script>

<style scoped>

.meme{
    height: 300px;
    display: flex;
    flex-direction: column;
    align-items:center;
    border: 1px solid grey;

}

.meme img {
    max-height: 200px;
    max-width: 250px;
}
</style>