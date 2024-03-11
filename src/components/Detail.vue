<template>
  <div>
    <h4>상세페이지</h4>
    <h5>
      {{ title }}
    </h5>
    <p>
      {{ content }}
    </p>
    <router-view> </router-view>
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
  data() {
    return {
      title: "",
      content: "",
    };
  },
  mounted() {
    const id = Number(this.$route.params?.id[0] ?? 0);
    console.log("[Mounted] id:", id);
    this.title = this.blogText?.[id]?.title ?? "No title";
    this.content = this.blogText?.[id]?.content ?? "No contents";
  },
};
</script>
<style></style>
