<template>
  <div id="app">
    <h1>BLOG</h1>

    <div v-for="(post, i) in postList" :key="'post_' + post.id" class="blog">
      <div style="display: flex">
        <div>
          {{ post.title }}
        </div>

        <div>
          <button @click="open(i)">OPEN</button>
        </div>
      </div>
      <div
        style="background-color: lightblue; padding: 10px"
        v-if="post.isOpen"
      >
        {{ post.body }}
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "App",
  components: {},

  data() {
    return {
      postList: [],
      msg: "",
    };
  },

  created() {
    this.initPosts();
  },

  methods: {
    initPosts() {
      axios
        .get("https://jsonplaceholder.typicode.com/posts")
        .then((response) => {
          console.log("response", response);

          let list = response.data.slice(0, 10);

          for (let i = 0; i < list.length; i++) {
            this.postList.push({
              ...list[i],
              isOpen: false,
            });
          }

          // this.postList = response.data.slice(0, 10);
        })
        .catch((error) => {
          console.error("error", error);
        });
    },

    open(index) {
      this.postList[index].isOpen = !this.postList[index].isOpen;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.blog {
  border: 1px solid black;
  margin: 10px;
}
</style>
