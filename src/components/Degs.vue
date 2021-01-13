<template>
  <div class="hello">
    <ul>
      <li v-for="exp in exps" :key="exp"><h1><span>{{ base }}</span><sup>{{ exp }}</sup> = {{ base ** exp }}</h1><hr /></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Degs",
  props: {
    base: Number,
    exps: Array,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
