<template>
  <div class="card-deck">
    <div v-bind:key="d.section" v-for="d in sections">
      <SectionItem v-bind:info="d" />
    </div>
  </div>
</template>

<script>
import SectionItem from './SectionItem.vue';

export default {
  name: "Sections",
  components: {
    SectionItem
  },
  props: ["sections"]
};
</script>