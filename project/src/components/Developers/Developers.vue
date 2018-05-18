<template>
  <ul>
    <li
      v-for="(developer, index) in developers"
      :key="index">
      <div>Name: {{ developer.name }}</div>
      <div>Framework: {{ developer.framework }}</div>
      <div>Description: {{ developer.description }}</div>
      <div>Salary: {{ developer.salary }}</div>
    </li>
  </ul>
</template>

<script>
import { events } from "../../main.js";
export default {
  data() {
    return {
      developers: [],
    }
  },
  methods: {
  },
  created() {
    fetch('https://developers-c2f70.firebaseio.com/developers.json')
      .then((response) => response.json())
      .then((data) => {
        this.developers = data;
      })
  }
}
</script>

<style>

</style>
