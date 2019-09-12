<template>
  <div class="outer">
    <div class="middle">
      <div class="inner">
        <GitHub/>
      </div>
    </div>
  </div>
</template>

<script>
import GitHub from './components/GitHub.vue'

export default {
  name: 'app',
  components: {
    GitHub
  }
}
</script>

<style>
html {
  margin: 0;
  padding: 0;

  height: 100vh;
  width: 100%;
}

body {
  background-color: rgb(14, 14, 14)
}

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

@media only screen and (max-width: 600px) {
  .inner {
    max-width: 200px;
  }
}
</style>
