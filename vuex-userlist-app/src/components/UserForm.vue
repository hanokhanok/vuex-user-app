<template>
  <div class="userform">
    <input type="text" placeholder="username"><br>
    <input type="text" placeholder="email"><br>
    <input type="text" placeholder="phone"><br>
    <div class="btn">
      <button>저장</button>
    </div>
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.userform {
  width: 60%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
input {
  width: 60%;
  height: 22%;
  border: none;
  border-bottom: 1px solid #ccc;
}
button {
  width: 70px;
  height: 30px;
  margin-top: 3px;
}
.btn {
  width: 100%;
  display: flex;
  justify-content: center;
}
</style>