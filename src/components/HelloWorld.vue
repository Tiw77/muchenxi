<template>
<div>
  <div class="info">
    <h2>Web Design</h2>
    <span>Muchenxi Tiw</span>
    
    <a href="javascript:;" @click="show()">Take a look</a>
    <img src="../assets/lufei.jpeg" />
  </div>
  <div class="popup" v-show="showPopup">
    <div class="tabs">
      <a class="tab" href="#div1">1</a>
      <a class="tab" href="#div2">2</a>
      <a class="tab" href="#div3">3</a>
    </div>

    <div id="div1" class="content">first</div>
    <div id="div2" class="content">second</div>
    <div id="div3" class="content">third</div>
  </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      showPopup: false
    }
  },
  methods: {
    show () {
      this.showPopup = true
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
  margin: 0;
  padding: 0;
}
a {
  text-decoration: none;
}

img,
h2,
span,
a {
  transition: all 1s;
}

div {
  box-sizing: border-box;
}
.info {
  width: 298px;
  height: 279px;
  border: 1px solid #ddd;
  margin: 50px auto;
  position: relative;
  overflow: hidden;
}
.info img {
  display: block;
  width: 100%;
  border: 0;

  margin: 0 auto;
  position: absolute;
}
.info:hover img {
  transform: scale(0.5);
}

h2 {
  font-size: 14px;
  font-weight: 900;
  position: absolute;
  top: 70px;
  left: 110px;
}

.info span {
  display: block;
  font-size: 11px;
  position: absolute;
  top: 95px;
  left: 110px;
}
.info a {
  padding: 4px;
  font-size: 12px;
  background: red;
  color: #fff;
  text-align: center;
  line-height: 26px;
  position: absolute;
  top: 155px;
  left: 110px;
}

.info:hover h2 {
  transform: translateY(-45px);
}
.info:hover span {
  transform: translateY(-48px);
}
.info:hover a {
  transform: translatey(68px);
}

.popup {
  box-sizing: border-box;
  width: 100%;
  height: 500px;
  position: absolute;
  top: 40px;
  left: 0;
  background: #E1DDF2;
  /* opacity: 0.8; */
  /* overflow: hidden; */
  overflow-y: auto;
  border: 1px solid #ddd;
  color: #000;
}

.tabs {
  margin-top: 20px;
  overflow: hidden;
  box-sizing: border-box;
  display: flex;
  justify-content: space-around;
}

.tab {
  float: left;
  width: 100px;
  height: 30px;
  line-height: 30px;
  text-align: center;
  color: #fff;
  background: #8779C8;
  opacity: 0.8;
  border-radius: 30px;
}

.content {
  margin-top: 20px;
  width: 100%;
  padding-left: 20px;
  box-sizing: border-box;
  height: 500px;
  text-align: left;
  font-size: 20px;
}
</style>
