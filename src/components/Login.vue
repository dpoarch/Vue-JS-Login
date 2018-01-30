<template>
  <div class="container">
    <form class="form-signin" @submit.prevent="login">
      <h2 class="form-signin-heading">Please sign in</h2>
      <label for="inputEmail" >Username</label>
      <input type="text" class="form-control" v-model="userName" required>
      <br>
      <label>Password</label>
      <input type="password" class="form-control" v-model="password" required>
      <br>
      <button class="btn btn-lg btn-primary btn-block" type="submit">Log In</button>
    </form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userName: "",
      password: ""
    };
  },
  methods: {
    login() {
      //write login authencation logic here!
      if (this.userName == "davidpoarch" && this.password == "qweqwe123") {
        localStorage.setItem("token", "ImLogin");
        this.$router.push("/");
      } else {
        alert("login failed");
        this.userName = "";
        this.password = "";
      }
    }
  }
};
</script>