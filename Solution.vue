<template>
  <table>
    <thead>
      <tr>
        <th>ID</th>
        <th>First Name</th>
        <th>Last Name</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="p in persons" :key="p.id">
        <td>{{ p.id }}</td>
        <td>{{ p.first_name }}</td>
        <td>{{ p.last_name }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
import { persons } from "./data";
export default {
  data() {
    return {
      persons,
    };
  },
};
</script>

<style>
table,
th,
td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>