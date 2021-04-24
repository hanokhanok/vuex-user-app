<template>
  <div class="register">
    <div class="form">
    <UserForm></UserForm>
    </div>
    <div class="list">
    <UserList></UserList>
    </div>
  </div>
</template>

<script>
import UserForm from '../components/UserForm.vue';
import UserList from '../components/UserList.vue';

export default {
  name: 'Register',
  components: {
    UserForm,
    UserList
  }
}
</script>

<style scoped>
.register {
  width: 100%;
  height: calc(100vh - 60px);
  display: flex;
  flex-wrap: wrap;
}
.form {
  width: 100%;
  height: 30%;
}
.list {
  width: 100%;
  height: 70%;
}
</style>