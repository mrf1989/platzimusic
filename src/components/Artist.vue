<template lang="pug">
  li
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    img(:src="artist.image[2]['#text']")
</template>

<script>
export default {
  name: 'artist',
  props: ['artist']
}
</script>

<style lang="stylus" scoped>
li
  display inline-block
  margin 10px
  border 2px solid #42b983
  padding 10px
  border-radius 10px
</style>
