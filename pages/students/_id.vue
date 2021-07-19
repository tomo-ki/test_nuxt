<template>
  <div class="student_id">
    <div v-for="student in students" :key="student.id">
      <h1 v-if="$route.params.id == student.id">{{student.name}}</h1>
    </div>
    <div class="links">
      <NuxtLink to="/students">生徒一覧へ戻る</NuxtLink>
      <div class="centerdiv">|</div>
      <NuxtLink to="/">トップページへ</NuxtLink>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  }
};
</script>


<style>
.student_id {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.links{
  display: flex;
}
.centerdiv{
  margin: 0 10px;
}
</style>