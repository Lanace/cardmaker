<template>
  <section>
    <h2>Preview</h2>
    <input id="file-input" type="file" v-on:change="fileLoad"/>
    <canvas id="canvas"></canvas>
  </section>
</template>

<script>
export default {
  data () {
    return {
      form: {},
      filePath: '',
      img: {},
      fr: {}
    }
  },
  methods: {
    fileLoad: function (event) {
      var file = event.target.files[0]
      this.fr = new FileReader()
      this.fr.onload = this.createImage
      this.fr.readAsDataURL(file)
    },
    createImage: function () {
      this.img = new Image()
      this.img.onload = this.imageLoaded
      this.img.src = this.fr.result
    },
    imageLoaded: function () {
      var canvas = document.getElementById('canvas')
      canvas.width = this.img.width
      canvas.height = this.img.height
      var ctx = canvas.getContext('2d')
      ctx.drawImage(this.img, 0, 0)
      alert(canvas.toDataURL('image/png'))
    }
  }
}
</script>

<style scoped>
</style>
