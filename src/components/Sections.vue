<template>
<div class="justify-content-center">
  <div class="card-deck ml-0">
    <div v-bind:key="d.section" v-for="d in sections">
      <SectionItem v-bind:info="d" />
    </div>
    <b-button v-b-modal.modal-1>Launch demo modal</b-button>

    <b-modal id="modal-1" title="BootstrapVue" centered hide-footer hide-header>
      <p class="my-4">Hello from modal!</p>
    </b-modal>
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