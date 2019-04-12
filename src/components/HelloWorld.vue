<template>
  <div>
    <div class="card"></div>
    <div class="card"></div>
    <div class="card"></div>
    <div class="card"></div>

    <!-- 固定宽高比例 -->
    <div aspectratio w-21-9>
      <div w-21-9-content></div>
    </div>
    <br>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* 基础使用 */
.card {
  margin: 30px auto;
  width: 90%;
  background-color: #eee;
  height: 300px;
}

[aspectratio] {
  position: relative;
}

[aspectratio]::before {
  content: '';
  display: block;
  width: 1px;
  margin-left: -1px;
  height: 0;
}

[aspectratio-content] {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
}

[w-21-9] {
  width: 90%;
  margin: 0 auto;
  background-color: #ccc;
}

[w-21-9] {
  aspect-ratio: '16:9';
}

[w-21-9-content] {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
}
</style>
