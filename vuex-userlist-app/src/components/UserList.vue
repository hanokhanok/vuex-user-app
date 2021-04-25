<template>
  <div class="userlist">
    <div class="grid">
      <div class="box" v-for="user in allUsers" :key="user.id">
        {{ user.title }}
        {{ user.username }}<br>
        {{ user.email }}<br>
        {{ user.phone }}
      </div>
    </div>
  </div>
</template>

<script>
import { mapGetters, mapActions } from "vuex"

export default {
  name: 'UserList',
  methods: {
    ...mapActions(['fetchUsers'])
  },
  computed: {
    ...mapGetters(['allUsers'])
  },
  created() {
    this.fetchUsers();
  }
}
</script>

<style scoped>
  .userlist{
    width: 100%;
    height: 100%;
    background-color: #ffffff;
  }
  .grid {
    display: grid;
    width: 80%;
    height: 100%;
    margin: 0 auto;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-gap: 7px;
  }
  .box {
    background-color: rgb(184, 218, 216);
    border-radius: 10px;
    padding-top: 5px;
    padding-left: 5px;
    color: rgb(43, 41, 41);
    font-size: 18px;
    line-height: 1.3;
  }
</style>