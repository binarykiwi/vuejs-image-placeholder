<template>
  <div id="app">
    <!-- Size -->
    <div>
      <label>
        <input v-model.number="width" type="number"> Width
      </label>
    </div>
    <div>
      <label>
        <input v-model="percentWidth" type="checkbox"> Width in percent?
      </label>
    </div>
    <div>
      <label>
        <input v-model.number="height" type="number"> Height
      </label>
    </div>
    <div>
      <label>
        <input v-model="percentHeight" type="checkbox"> Height in percent?
      </label>
    </div>
    <!-- Display -->
    <div>
      <label>
        <input v-model.number="showRatio" type="checkbox"> Show Ratio?
      </label>
    </div>
    <!-- Styling -->
    <div>
      <label>
        <input v-model="backgroundColor"> Background Color
      </label>
    </div>
    <div>
      <label>
        <input v-model="borderColor"> Border Color
      </label>
    </div>
    <div>
      <label>
        <input v-model.number="borderWidth" type="number"> Border Width
      </label>
    </div>
    <!-- Typography -->
    <div>
      <label>
        <input v-model="fontFamily"> Font Family
      </label>
    </div>
    <div>
      <label>
        <input v-model="fontColor"> Font Color
      </label>
    </div>
    <div>
      <label>
        <input v-model.number="fontSize" type="number"> Font Size (px)
      </label>
    </div>
    <!-- External Styling -->
    <div>
      <label>
        <input v-model="class"> CSS Class Name
      </label>
    </div>
    <!-- Image Placeholder -->
    <div>
      <image-placeholder
        :width="width"
        :percentWidth="percentWidth"
        :percentHeight="percentHeight"
        :height="height"
        :show-ratio="showRatio"
        :background-color="backgroundColor"
        :border-color="borderColor"
        :border-width="borderWidth"
        :font-family="fontFamily"
        :font-color="fontColor"
        :font-size="fontSize"
        :class="mycustomclass"
      ></image-placeholder>
    </div>
  </div>
</template>
<script>
import ImagePlaceholder from './components/ImagePlaceholder'
export default {
  components: {
    ImagePlaceholder
  },
  data () {
    return {
      width: 300,
      height: 200,
      percentWidth: false,
      percentHeight: false,
      showRatio: false,
      backgroundColor: '#eee',
      borderWidth: 1,
      borderColor: '#ccc',
      fontFamily: 'Helvetica, sans-serif',
      fontColor: '#333',
      fontSize: 14
    }
  }
}
</script>
