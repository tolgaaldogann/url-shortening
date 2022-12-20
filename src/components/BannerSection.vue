<template>
    <div class="banner">
      <div class="content">
        <div class="text">
          <div>
            <h1 class="title">
              More than just <br />
              shorter links
            </h1>
            <span class="banner-text"
              >Build your brand's recognition and get detailed <br />
              insights on how your links are performing.</span
            ><br />
            <button class="btn">Get Started</button>
          </div>
          <img
            class="illustration-working"
            src="../assets/illustration-working.svg"
            alt=""
          />
        </div>
      </div>
    </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.banner {
  display: flex;
  flex-direction: column;
  padding: 40px 150px 100px 150px;
}
.text {
  display: flex;
  justify-content: space-between;
}
.illustration-working {
  width: 300px;
}
.title {
  font-weight: 900;
  line-height: 35px;
  font-size: 36px;
  margin-bottom: 10px;
}
.banner-text {
  color: #9b9a9f;
}
.btn {
  background: #2bd1d1;
  color: #fff;
  border: none;
  margin-top: 20px;
  padding: 8px 12px;
  border-radius: 20px;
}
.statistics{
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 50px;
  border-radius: 10px;
  position: relative;
  background: #F0F1F6;
}
.shorten-link-input{
  width: 100%;
  display: flex;
  justify-content: center;
  position: absolute;
  background: #4B406B;
}
.input{
  width:500px;
  height: 25px;
  border-radius:10px;
  padding: 10px;
  margin-right: 10px;
}
.btn-shorten{
  background: #2bd1d1;
  color: #fff;
  border: none;
  padding: 0 30px;
  border-radius: 20px;
}
</style>
