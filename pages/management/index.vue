<template>
  <div class="management">
    <h1>生徒管理ページ</h1>
    <table class="management__table">
      <tr>
        <th>名前</th>
        <th>ID</th>
      </tr>
      <tr v-for="student in students" :key="student.id">
        <td class="management__table-name">{{ student.name }}</td>
        <td class="management__table-id">{{ student.id }}</td>
      </tr>
    </table>
    <NuxtLink to="/">戻る</NuxtLink>
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
  },
};
</script>


<style>
.management {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.management__table tr{
  height: 60px;
}
.management__table{
  width: 35%;
  margin-bottom: 30px;
}
.management__table-name{
  width: 40%;
}
</style>
