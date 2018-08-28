<template>
  <section>
    <preview></preview>
    <image-option-box></image-option-box>
    <text-option-box></text-option-box>
  </section>
</template>

<script>
import ImageOptionBox from '@/components/ImageOptionBox.vue'
import Preview from '@/components/Preview.vue'
import TextOptionBox from '@/components/TextOptionBox.vue'

export default {
  data () {
    return {}
  },
  components: {ImageOptionBox, TextOptionBox, Preview}
}
</script>

<style scoped>

</style>
