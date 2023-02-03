<template>
  <div class="login-container">
    <div class="header">
      <img src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png" alt="Google Logo" />
    </div>
    <form>
      <div class="form-group">
        <label for="username">Username</label>
        <input v-model="username" type="text" id="username" />
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input v-model="password" type="password" id="password" />
      </div>
      <div class="form-group">
        <button @click="submit">Sign in</button>
      </div>
    </form>
  </div>
</template>

<style>
.login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 40px;
}

.header {
  margin-bottom: 40px;
}

.form-group {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 20px;
}

label {
  font-size: 14px;
  margin-bottom: 10px;
}

input {
  width: 300px;
  height: 40px;
  padding: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  width: 300px;
  height: 40px;
  background-color: #4285f4;
  color: #fff;
  font-size: 16px;
  border-radius: 4px;
  border: none;
  cursor: pointer;
}
</style>

<script>
export default {
  data() {
    return {
      username: "",
      password: ""
    };
  },
  methods: {
    submit() {
      // make a request to the server with the username and password
      console.log(`Username: ${this.username} Password: ${this.password}`);
    }
  }
};
</script>



