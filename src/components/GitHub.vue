<template>
  <div>
    <a href="https://github.com/muazamkamal/mmrtracker"><img id="gh-logo" alt="GitHub logo" src="../assets/gh-logo.svg"></a>
  </div>
</template>

<script>
export default {
  name: 'GitHub'
}
</script>

<style scoped>
#gh-logo {
  max-width: 100%;
  height: auto;
  width: auto\9; /* ie8 */

  display: block;
  margin: 0 auto;

  -webkit-filter: invert(.8); /* safari 6.0 - 9.0 */
  filter: invert(.8);
}

#gh-logo:hover {
  -webkit-filter: invert(1); /* safari 6.0 - 9.0 */
  filter: invert(1);
}
</style>
