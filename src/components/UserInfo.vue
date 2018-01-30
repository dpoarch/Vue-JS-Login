<template>
<div class="container">
    <h1>User Information</h1>
    <h3>ID:</h3>
    <p>{{ userId }}</p>
    <h3>Username:</h3>
    <p>{{ userName }}</p>
    
  </div>
</template>
<script>
export default {
  data() {
    return {
      userName: "David Poarch",
      userId: "0001"
    };
  }
};
</script>