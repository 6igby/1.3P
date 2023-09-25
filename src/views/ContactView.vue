<template>
  <div>
    <h1>Contact Me</h1>
    <form @submit.prevent="submitForm">
      <div>
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="formData.name" required>
      </div>
      <div>
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="formData.email" required>
      </div>
      <div>
        <label for="message">Message:</label>
        <textarea id="message" v-model="formData.message" required></textarea>
      </div>
      <button type="submit">Submit</button>
    </form>

    <div v-if="submitted">
      <h3>Thank you for your message!</h3>
    </div>
  </div>
</template>

<script style>
  export default {
  data() {
    return {
      formData: {
        name: '',
        email: '',
        message: ''
      },
      submitted: false
    };
  },
  methods: {
    submitForm() {
      this.formData = {
        name: '',
        email: '',
        message: ''
      };
      this.submitted = true;
    }
  }
};
</script>

<style lang="scss" scoped>
  @import url(../assets/ContactView.css);
</style>

