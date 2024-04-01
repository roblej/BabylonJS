<template>

<div>
  <h3>Babylone Examples</h3>
  <canvas></canvas>
</div>
<button>Click me!</button>

</template>

<script lang="ts">
import { defineComponent } from 'vue';
// import {BasicScene} from '@/BabylonExamples/BasicScene'
import {StandardMaterials} from "@/BabylonExamples/StandardMaterials"
export default defineComponent({
  name: 'BabylonExamples',
  mounted(){
    const canvas = document.querySelector("canvas")!;
    // new BasicScene(canvas);
    new StandardMaterials(canvas)
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

canvas{
  width:70%;
  height:70%;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
