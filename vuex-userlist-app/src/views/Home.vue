<template>
  <div class="home">
    <div class="ex">
    <p>Vue.js를 이용한 회원관리 app</p>
    <span>list 메뉴를 클릭하고 회원을 확인하세요!</span>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.home {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
}

.ex {
  margin: 0 auto;
  width: 60%;
  height: 60px;
  line-height: 60px;
  text-align: center;
}

.ex p {
  font-size: 24px;
  font-weight: bold;
}
</style>