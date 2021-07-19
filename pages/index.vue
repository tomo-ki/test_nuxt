<template>
  <div class="container">
    <div class="container__left">
      <h1>生徒情報</h1>
      <NuxtLink to="/students">生徒の情報を見る</NuxtLink>
    </div>
    <div class="container__right">
      <h1>管理者</h1>
      <NuxtLink to="/management">管理画面を見る</NuxtLink>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.container__left, .container__right{
  margin: 30px;
}
</style>