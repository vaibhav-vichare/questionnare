<template>
  <div class="component-wrapper">
    <Information />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Information from "@/components/Information.vue";

@Options({
  components: {
    Information,
  },
})
export default class HomeView extends Vue {}
</script>
