<template>
  <div class="outer">
    <div class="middle">
      <div class="inner">
        <a href="https://github.com/muazamkamal/mmrtracker"><img id="gh-logo" alt="GitHub logo" src="../assets/gh-logo.svg"></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'GitHub'
}
</script>

<style scoped>
/*
  Triple div method of centering
  obtain at https://stackoverflow.com/a/6182661/5635689
*/
.outer {
  display: table;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}

.middle {
  display: table-cell;
  vertical-align: middle;
}

.inner {
  margin-left: auto;
  margin-right: auto;
  width: 300px;
  max-width: 300px;
}

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
