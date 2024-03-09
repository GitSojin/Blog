<template>
  <div>
    <h4>상세페이지</h4>
    <h5>{{ blogText[$route.params.id].title }}</h5>
    <p>{{ blogText[$route.params.id].content }}</p>
  </div>

  <div class="card" style="width: 18rem">
    <img src="./lucky3.jpg" class="card-img-top" alt="KimLucky" />
    <div class="card-body">
      <p class="card-text">230524 럭키랑 피크닉 ☀️</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "Detail",
  props: {
    blogText: Array,
  },
};
</script>
<style></style>
