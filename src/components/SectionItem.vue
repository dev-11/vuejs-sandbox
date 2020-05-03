<template>
  <div>
    <div class="card mb-3" style="max-width: 600px;">
      <div class="card-header">{{info.section}}</div>
      <div class="row no-gutters">
        <div class="col-md-4">
          <img v-bind:src="info.img" class="card-img-top" alt="asdf" />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <div class="card-text">{{ info.title }} by {{ info.authors }}</div>
            <div class="card-text">{{ info.price }} | {{ info.format }}</div>
            <hr class="mt-3 mb-3 ml-5 mr-5" />
            <div class="card-text text-justify">{{ info.desc }}
            </div>
          </div>
        </div>
      </div>
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
/* h1 {
  color: #f0f7f4;
} */

/* .lighten {
  color: white;
} */
</style>
