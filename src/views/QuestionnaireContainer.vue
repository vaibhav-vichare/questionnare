<template>
  <div class="component-wrapper">
    <div v-for="(question, index) in questionsData" :key="index">
      <Questions :question="question" />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Questions from "@/components/Questions.vue";
import QuestionnaireData from "../assets/questionnaire.json";

@Options({
  components: {
    Questions,
  },
})
export default class QuestionnaireContainer extends Vue {
  data() {
    return {
      questionsData: QuestionnaireData.questionnaire.questions,
    };
  }
}
</script>
