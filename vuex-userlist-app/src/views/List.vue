<template>
  <div class="userli">
    <div class="list">
    <UserList></UserList>
    </div>
  </div>
</template>

<script>
import UserList from '../components/UserList.vue';

export default {
  name: 'List',
  components: {
    UserList
  }
}
</script>

<style scoped>
.userli {
  width: 100%;
  height: calc(100vh - 60px);
  display: flex;
  flex-wrap: wrap;
}
.list {
  width: 100%;
  height: 100%;
  padding-top: 40px;
}
</style>