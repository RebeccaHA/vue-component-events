<template>
  <div>
    <user-data @data-input="setData"></user-data>
    <active-user :name="this.name" :age="this.age"></active-user>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      age: null
    };
  },
  methods: {
    setData(name, age) {
      this.name = name;
      this.age = age;
    }
  }
};
</script>