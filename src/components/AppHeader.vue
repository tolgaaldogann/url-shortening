<template>
  <div class="navbar">
    <div class="links">
      <span class="logo">Shortly</span>
      <ul class="link">
        <li>Features</li>
        <li>Pricing</li>
        <li>Resources</li>
      </ul>
    </div>
    <div class="button-wrapper">
      <button class="btn-login">Login</button>
      <button class="btn-sign">Sign Up</button>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar{
  display: flex;
  justify-content: space-between;
  padding: 40px 150px;
}
.links{
  display: flex;
  align-items: center;
}
.logo{
  font-size: 24px;
  font-weight: 700;
  color: #323139;
  cursor: pointer;
}
.link {
  display: flex;
  list-style-type: none;
  margin: 0;
}
li{
  margin-left: 20px;
  cursor: pointer;
  color: #ACABB1;
  font-size: 12px;
}
.button-wrapper{
  display: flex;
  justify-content: center;
  align-items: center;
}
.btn-login{
  background: transparent;
  border: none;
  color: #919095;
}
.btn-sign{
  background: #2FCED0;
  margin-left: 20px;
  border-radius: 20px;
  border: none;
  color: #fff;
  padding: 10px 15px;
}
</style>
