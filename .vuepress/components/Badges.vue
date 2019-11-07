<template>
  <span>
    <img alt="GitHub stars" :src="'https://img.shields.io/github/stars/'+fullRepo" />
    <img alt="GitHub contributors" :src="'https://img.shields.io/github/contributors/'+fullRepo" />
    <img alt="GitHub last commit" :src="'https://img.shields.io/github/last-commit/'+fullRepo" />
  </span>
</template>
<script>
export default {
  props: ["user", "repo"],
  computed: {
    fullRepo() {
      return this.user + "/" + this.repo;
    }
  }
};
</script>
