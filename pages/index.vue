import Vue from 'vue';
import VueAnalytics from 'vue-analytics';

// Configuration VueAnalytics
Vue.use(VueAnalytics, {
  id: 'UA-175589537-1'
});
<template>
  <div>
    <hero-section />
    <div class="container mx-auto flex justify-center space-x-4">
      <button-twitter />
      <button-facebook />
    </div>
    <template-section :cards="cards" />
    <LayoutFooter />
  </div>
</template>

<script>
export default {
  components: {
    HeroSection: () => import("./-HeroSection"),
    TemplateSection: () => import("./-TemplateSection"),
  },
  asyncData() {
    const { templates } = require("@/static/data/templates.json")
    return {
      cards: templates,
    }
  },
}
</script>

<style scoped></style>
