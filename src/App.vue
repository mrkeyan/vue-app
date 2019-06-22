<template>
  <div id="app" class="small-container">
    <h1>Employees</h1>
    <employee-table :employees="employees" />
  </div>
</template>

<script>
/*  original example, rename to app.vue to get it to work */
import EmployeeTable from '@/components/EmployeeTable.vue'

export default {
  name: 'app',
  components: {
    EmployeeTable,
  },
  data(){
    return {
      employees: [
        {
          id: 1,
          name: 'Richard Hendricks',
          email: 'richard@piedpiper.com',
        },
        {
          id: 2,
          name: 'Bertram Gilfoyle',
          email: 'bertram@gilfoyle.com',
        },
        {
          id: 3,
          name: 'Dinesh Chugtai',
          email: 'dinesh@chugtai.com',
        },
      ],
    }
  },
}
</script>

<style>
button {
  background: #009435;
  border: 1px solid #009435;
}

.small-container {
  max-width: 680px;
}
</style>
