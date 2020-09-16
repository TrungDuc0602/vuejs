<template>
  <div class="list-user">
    <user class="user" v-for="user in listUser" v-bind:key="user.id" v-bind:user="user" />
  </div>
</template>

<script>
import User from "./User.vue";
export default {
  name: "list-user",
  props: {
    titleHeader: String,
    listUser: {
      type: Array,
      default: [],
    },
  },
  data() {
    return {};
  },
  components: {
    User,
  },
};
</script>

<style>
.list-user {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.list-user .user {
  padding: 30px;
  margin-bottom: 30px;
  border: 1px solid black;
  width: calc(33.3333% - 20px);
}
</style>