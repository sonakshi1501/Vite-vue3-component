<script >
export default {
  data() {
    return {
      posts: [],
    };
  },
  mounted() {
    this.getAllPosts();
  },
  methods: {
    getAllPosts() {
      fetch("https://api.github.com/users")
        .then((res) => res.json())
        .then((data) => {
          console.log(data);
          this.posts = data;
        })
        .catch((e) => {
          console.log(e);
        });
    },
  },
};
</script>

<template>
  <!-- {{posts}} -->
  <div class="container m-0 p-0">
    <div class="row">
      <div class="col-md-4 mb-2" v-for="(post, index) in posts" :key="index">
        <div class="card">
          <img :src="post.avatar_url" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">{{ post.login }}</h5>
            <a :href="post.html_url" class="btn btn-primary">Click Me</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>
