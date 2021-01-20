<template>
  <div>
    <input type="text" v-model="name" />
    <input type="text" v-model="age" />
    <button type="submit" @click="submitData">Submit</button>
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
    submitData() {
      this.$emit("data-input", this.name, this.age);
    }
  }
};
</script>