<template>
  <section id="home-section">
    <preview id="priview-section"></preview>
    <div>
      <image-option-box></image-option-box>
      <text-option-box></text-option-box>
    </div>
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

#home-section {
  display: flex;
  flex-direction: row;
}

#priview-section {
  flex-grow: 1;
}

</style>
