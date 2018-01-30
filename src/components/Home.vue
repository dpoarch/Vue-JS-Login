<template>
<div class="container">
  <h1>Home</h1>
  <h2>Hello {{userName}}!</h2>  
</div>
</template>

<script>
export default {
  data() {
    return {
      userName: "David Poarch"
    };
  }
};
</script>