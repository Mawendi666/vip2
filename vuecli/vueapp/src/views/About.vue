<template>
  <div class="about">
    <h1>This is an about page</h1>
    <router-link to="/about/childone">子页面1</router-link>
    <router-link to="/about/childtwo">子页面2</router-link>
    <router-view/>
  </div>
</template>
<script>
export default {
  beforeRouteEnter (to, from, next) {
    // console.log(to, from)
    next();
  },
  beforeRouteLeave (to, from, next) {
    // console.log(to, from);
    next();
  }
}
</script>