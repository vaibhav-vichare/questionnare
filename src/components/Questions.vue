<template>
  <div class="card-component">
    <div class="title">{{ headline }}</div>
    <div class="description">{{ description }}</div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
@Options({
  props: {
    question: Object,
  },
})
export default class Questions extends Vue {
  question!: any;
  data() {
    return {
      headline: this.question.headline,
      description: this.question.description,
    };
  }
}
</script>

<style scoped lang="scss">
@import "../assets/styles/common.scss";
.card-component {
  box-shadow: 0 4px 3px -2px rgb(0 0 0 / 20%), 0 2px 2px 0 rgb(0 0 0 / 14%),
    0 1px 5px 0 rgb(0 0 0 / 12%);
  border-radius: $building-unit;
  padding: $building-unit-x5;
  margin: $building-unit-x5;
  border-width: thin;
  border-color: $border-color;
  .title {
    font-size: $font-size-18;
    font-weight: 600;
    padding: $building-unit 0 $building-unit-x3 0;
  }
  .description {
    font-size: $font-size-16;
    padding: $building-unit 0 $building-unit-x3 0;
  }
}
</style>
