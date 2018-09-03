<template>
  <section>
    <b-form>
      <b-form-group label="Brightness:" label-for="image-brightness-input" description="Brightness is brightness">
        <b-form-input id="image-brightness-input" type="range" v-model="imageOption.brightness" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Contrast:" label-for="image-contrast-input" description="Contrast is contrast">
        <b-form-input id="image-contrast-input" type="range" v-model="imageOption.contrast" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Saturation:" label-for="image-saturation-input" description="Saturation is saturation">
        <b-form-input id="image-saturation-input" type="range" v-model="imageOption.saturation" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Vibrance:" label-for="image-vibrance-input" description="Vibrance is vibrance">
        <b-form-input id="image-vibrance-input" type="range" v-model="imageOption.vibrance" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Hue:" label-for="image-hue-input" description="Hue is hue">
        <b-form-input id="image-hue-input" type="range" v-model="imageOption.hue" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Sepia:" label-for="image-sepia-input" description="Sepia is sepia">
        <b-form-input id="image-sepia-input" type="range" v-model="imageOption.sepia" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Gamma:" label-for="image-gamma-input" description="Gamma is gamma">
        <b-form-input id="image-gamma-input" type="range" v-model="imageOption.gamma" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Noise:" label-for="image-noise-input" description="Noise is noise">
        <b-form-input id="image-noise-input" type="range" v-model="imageOption.noise" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Clip:" label-for="image-clip-input" description="Clip is clip">
        <b-form-input id="image-clip-input" type="range" v-model="imageOption.clip" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="Sharpen:" label-for="image-sharpen-input" description="Sharpen is sharpen">
        <b-form-input id="image-clip-sharpen" type="range" v-model="imageOption.sharpen" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>

      <b-form-group label="StackBlur:" label-for="image-stackblur-input" description="StackBlur is stackBlur">
        <b-form-input id="image-stackblur-sharpen" type="range" v-model="imageOption.stackBlur" v-on:change="optionChanged()"></b-form-input>
      </b-form-group>
    </b-form>
  </section>
</template>

<script>
var imageOption = {}

export default {
  data () {
    return {
      imageOption: imageOption
    }
  },
  methods: {
    optionChanged: function () {
      console.log(imageOption)
    }
  }
}
</script>

<style scoped>

</style>
