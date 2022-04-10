<template>
  <div class="information">
    <h1>Questionnaire information</h1>
    <h2>Concepts:</h2>
    <ul>
      <li>
        <div>Questionnaire</div>
        <ul>
          <li>A Questionnaire has a title and a description</li>
          <li>
            A questionnaire has a defined sequence of question that need to be
            answered
          </li>
        </ul>
      </li>
      <li>
        <div>Question</div>
        <ul>
          <li>
            3 different types of questions are supported: Freetext, Multiple
            choice (single answer), Multiple choice (multi answer)
          </li>
          <li>
            For Multiple Choice, each choice has a descriptive label that is
            shown to the user
          </li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
  },
})
export default class HelloWorld extends Vue {
  msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/styles/common.scss";
</style>
