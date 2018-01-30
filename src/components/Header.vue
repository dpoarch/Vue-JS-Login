<template>
  <!-- <div>
    <router-link to="/">Home</router-link>
    <router-link to="/userInfo">User Info</router-link>
    <a href="" @click.prevent="logout">Logout</a>
  </div> -->

  <nav class="navbar navbar-default">
    <div class="container-fluid">
        <div class="navbar-header">
          <a class="navbar-brand" href="#">Vue Login</a>
        </div>
      <ul class="nav navbar-nav">
      <li ><router-link to="/">Home</router-link></li>
      <li class={}><router-link to="/userInfo">User Info</router-link></li>
      <li><a href="" @click.prevent="logout">Logout</a></li>
    </ul>
  </div>
  </nav>
</template>




<script>
export default {
  methods: {
    logout() {
      localStorage.removeItem("token");
      this.$router.push("/login");
    }
  }
};
</script>