<template>
  <div>
    <h1>{{info.section}}</h1>

    <img v-bind:src="info.img" />
    <div>
      {{ info.authors }}:
      <span class="lighten">{{ info.title }}</span>
    </div>

    <div>
      Price:
      <span class="lighten">{{ info.price }}</span>
    </div>

    <div>
      Format:
      <span class="lighten">{{ info.format }}</span>
    </div>

    <div>
      Description:
      <span class="lighten">{{ info.desc }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionItem",
  props: {
    info: Object
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #f0f7f4;
}

.lighten {
  color: white;
}
</style>
