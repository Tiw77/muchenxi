<template>
<div>
  <h2>Web Design</h2>
  <span>Muchenxi Tiw</span>
  
  <a href="#">Take a look</a>
  <img src="../assets/lufei.jpeg" />
</div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
    }
  }
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
  width: 298px;
  height: 279px;
  border: 1px solid #ddd;
  margin: 50px auto;
  position: relative;
  overflow: hidden;
}
div img {
  display: block;
  width: 100%;
  border: 0;

  margin: 0 auto;
  position: absolute;
}
div:hover img {
  transform: scale(0.5);
}

h2 {
  font-size: 14px;
  font-weight: 900;
  position: absolute;
  top: 70px;
  left: 110px;
}

span {
  display: block;
  font-size: 11px;
  position: absolute;
  top: 95px;
  left: 110px;
}
a {
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

div:hover h2 {
  transform: translateY(-45px);
}
div:hover span {
  transform: translateY(-48px);
}
div:hover a {
  transform: translatey(68px);
}
</style>
