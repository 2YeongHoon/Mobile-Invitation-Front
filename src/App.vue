<template>
  <div class="login-page">
    <div class="login-container">
      <h2>모바일 청첩장</h2>

      <form>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="email" required>
        </div>

        <div class="form-group">
          <label for="password">Password:</label>
          <input type="password" id="password" v-model="password" required>
        </div>

        <div class="form-group">
          <button type="submit">Submit</button>
        </div>

        <div class="form-group">
          <button type="button" @click="forgotPassword()">Forgot password?</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      password: '',
    };
  },
  methods: {
    forgotPassword() {
      // Implement your password retrieval logic here
    },
  },
};
</script>

<style scoped>
.login-page {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.login-container {
  width: 350px;
  padding: 30px;
  border: 1px solid #2196f3;
}

form {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-group {
  margin: 10px 0;
}

label {
  margin-right: 10px;
}

input {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-sizing: border-box;
  margin-bottom: 10px;
}

button[type="submit"] {
  background-color: #2196f3;
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: #0c7cd5;
}

button[type="button"] {
  background-color: transparent;
  color: #2196f3;
  border: none;
  cursor: pointer;
}
</style>
