<template>
  <div>
    <h1>This is End Page!!</h1>
    <div class="end-page">
      <router-view/>

      <div class="container">My name is aaaa.</div>
    </div>
  </div>
</template>

<script>
/*
export default {
}
*/
</script>

<style>
.end-page {
  border: 1px dotted #4e2424;
  width: 100vw;
  padding: 20px;
}
</style>