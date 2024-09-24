<script setup>

import { onMounted } from 'vue';

const url = 'http://localhost/wordpress_2023-2024/wp-json/wp/v2/posts';

onMounted(() => {
  console.log('mounted');
  fetch(url)
  .then(response => response.json())
  .then(data => console.log(data)); 

});
</script>


<template>
    Ciao Mimi Bibi
</template>