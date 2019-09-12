<template>
  <div>
    <div class="outer">
      <div class="middle">
        <div class="inner">
          <GitHub/>
        </div>
      </div>
    </div>
    <div class="footer">
      <a href="https://github.com/muazamkamal/mmrtracker-web" @mouseover="hover = true" @mouseleave="hover = false" class="source-text"><span v-if="hover">[ Source Code ]</span><span v-else>Source Code</span></a>
    </div>
  </div>
</template>

<script>
import GitHub from './components/GitHub.vue'

export default {
  name: 'app',
  components: {
    GitHub
  },
  data () {
    return {
      hover: false
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto+Condensed');

html {
  margin: 0;
  padding: 0;

  height: 100vh;
  width: 100%;

  font-family: 'Roboto Condensed', sans-serif;
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

.footer {
  display: flex;
  position: absolute;
  width: 100%;
  bottom: 10px;
  left: 0;
}

.source-text {
  margin: 0 auto;
  text-decoration: none;
  text-align: center;
  color: white;
}
</style>
