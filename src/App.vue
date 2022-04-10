<template>
  <header>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/QuestionnaireContainer"
        >Go to Questionnaire</router-link
      >
    </nav>
  </header>
  <router-view />
</template>

<style lang="scss">
@import "assets/styles/common.scss";
</style>
