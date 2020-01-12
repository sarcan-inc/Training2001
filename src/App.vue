<template>
  <div>
    <MyHeader>
      <nav id="glnav">
        <ul>
          <li @click="currentComponent = 'Home'">Home</li>
          <li @click="currentComponent = 'About'">About</li>
          <li @click="currentComponent = 'Blog'">Blog</li>
          <li @click="currentComponent = 'Inquiry'">Inquiry</li>
        </ul>
      </nav>
    </MyHeader>
    <component v-bind:is="currentComponent"></component>
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import Home from "./components/Home.vue";
import About from "./components/About.vue";
import Inquiry from "./components/Inquiry.vue";
import Blog from "./components/Blog.vue";

export default {
  data: function() {
    return {
      currentComponent: "Home"
    };
  },
  components: {
    MyHeader,
    Home,
    About,
    Inquiry,
    Blog
  }
};
</script>

<style>
h2 {
  padding: 10px;
  background-color: #eee;
  fint-size: 18px;
  line-height: 1;
}
</style>
