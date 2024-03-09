<template>
  <div>
    <h5>{{ blogText[0].title }}</h5>
    <p>Today : {{ blogText[0].date }}</p>
  </div>
  <div>
    <h5>{{ blogText[1].title }}</h5>
    <p>Today : {{ blogText[1].date }}</p>
  </div>
  <div>
    <h5>{{ blogText[2].title }}</h5>
    <p>Today : {{ blogText[2].date }}</p>
  </div>
</template>
<script>
export default {
  name: "list",
  props: {
    blogText: Object,
  },
};
</script>
<style></style>
