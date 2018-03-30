<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
html {
  background-color: #0e3667;
}
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
.el-select .el-input__inner {
  width: 2.55rem;
  height: .8rem;
  font-size: .4rem;
}
.mt-range {
  height: .5rem !important;
  line-height: .5rem !important;
}
.parameter .mt-range{
  width: 2.55rem;
}
.mt-range .mt-range-thumb {
  border-radius: 0;
  width: .6rem;
  height: .4rem ;
  top: 0.05rem;
  /* background-color: #20a0ff; */
  border-left: .3rem solid #20a0ff;
  background-color: transparent;
  box-shadow: none;
}
.mt-range .mt-range-content {
  margin-right: .3rem;
}
.mt-range .mt-range-runway {
  border-top-width: .08rem !important;
  border-image-source: url('../static/bg_line.png');
  border-image-width: 100% 100% 0% 0%;
  border-image-repeat: round;
  width: calc(100% + .3rem);
}
.mt-range .mt-range-progress {
  background-color: #3a88bf;
  height: .08rem !important;
}

.el-table .cell {
  line-height: normal;
}

.system_content_css .mt-range .mt-range-runway {
  width: calc(100% + .3rem);
}
</style>
