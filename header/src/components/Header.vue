<template>
<div class="header">
  <h1 class="header__title">Приложение "Хэдер"</h1>
</div>
</template>

<script>
export default {
name: "Header"
}
</script>

<style scoped>
.header {
  height: 100px;
  background-color: #091F52;
  display: flex;
  align-items: center;
  justify-content: start;
}
.header__title {
  margin-left: 5px;
  color: #FFFFFF;
}
</style>