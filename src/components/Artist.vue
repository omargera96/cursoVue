<template lang="pug">
  li
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    a(:href="artist.url" target="_blank"): img(:src="artist.image[2]['#text']") 
</template>

<script>
export default {
  name: 'artist',
  props: [ 'artist' ]
}
</script>

<style lang="stylus" scoped>
li
  display inline-block
  margin 10px
  border 2px solid #41b883
  padding 5px
  
img 
  border-radius 20px
</style>
