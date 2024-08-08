
<template>
  <div>
    <ol class="employee-list">
      <li v-for="employee in employees" :key="employee.name">
        {{ employee.name }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  name: 'EmployeeList',
  data() {
    return {
      employees: [
        { name: 'Mohamed  Bankolé' },
        { name: 'Aichettou Gaye' },
        { name: 'Mohamed Soumaré' },
        { name: 'Harouna Traoré' },
        { name: 'Thillo Sem' }
      ]
    };
  }
};
</script>

<style scoped>
.employee-list {
  list-style-type: none;
  padding: 0;
}

.employee-list li {
  padding: 20px;
  margin: 5px 0;
  border: 2px solid #ddd;
  border-radius: 5px;
  cursor: pointer;
}

.employee-list li:hover {
  background-color: #f0f0f0;
}

</style>
