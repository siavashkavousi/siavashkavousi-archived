<template>
  <a :href="src">
    <img src="../assets/github-logo.svg" width="20">
  </a>
</template>

<script>
  export default {
    props: {
      src: String
    }
  }
</script>
