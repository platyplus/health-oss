<template>
  <span>
    <img class="badge" alt="GitHub stars" :src="'https://img.shields.io/github/stars/'+fullRepo" />
    <img
      class="badge"
      alt="GitHub contributors"
      :src="'https://img.shields.io/github/contributors/'+fullRepo"
    />
    <img
      class="badge"
      alt="GitHub last commit"
      :src="'https://img.shields.io/github/last-commit/'+fullRepo"
    />
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

<style lang="stylus" scoped>
.badge {
  display: inline-block;
  font-size: 14px;
  height: 18px;
  line-height: 18px;
  border-radius: 3px;
  color: white;

  & + & {
    margin-left: 5px;
  }
}
</style>