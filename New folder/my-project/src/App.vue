<template class ='container'>
  <div id="app">
    <div class="container">
      <comp-header v-bind:titleHeader="title" />
      <list-user v-bind:listUser="listUser" />
    </div>
  </div>
</template>

<script>
import ListUser from "./components/ListUser.vue";
import CompHeader from "./components/CompHeader.vue";
export default {
  name: "app",
  data() {
    return {
      title: "Hello, how are u?",
      listUser: [
        { id: 100, email: "100@gmail.com", isactive: true },
        { id: 101, email: "101@gmail.com", isactive: false },
        { id: 102, email: "102@gmail.com", isactive: true },
        { id: 103, email: "103@gmail.com", isactive: false },
        { id: 104, email: "104@gmail.com", isactive: false },
        { id: 105, email: "105@gmail.com", isactive: true },
        { id: 106, email: "100@gmail.com", isactive: true },
        { id: 107, email: "101@gmail.com", isactive: false },
        { id: 108, email: "102@gmail.com", isactive: true },
        { id: 109, email: "103@gmail.com", isactive: false }
      ],
    };
  },
  components: {
    CompHeader,
    ListUser,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.container {
  max-width: 1170px;
  margin: 0 auto;
  padding: 0 15px;
  min-height: 3000px;
}
</style>
