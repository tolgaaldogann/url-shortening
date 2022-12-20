<template>
    <div class="footer">
      <div class="logo">
        Shortly
      </div>
      <div class="links">
        <div class="link">
          <span class="title">Features</span>
          <ul>
            <li>Link Shortening</li>
            <li>Branded Links</li>
            <li>Analytics</li>
          </ul>
        </div>
        <div class="link">
          <span class="title">Resources</span>
          <ul>
            <li>Blog</li>
            <li>Developers</li>
            <li>Support</li>
          </ul>
        </div>
        <div class="link">
          <span class="title">Company</span>
          <ul>
            <li>About</li>
            <li>Our Team</li>
            <li>Careers</li>
            <li>Contact</li>
          </ul>
        </div>
      </div>
      <div class="social">
        <img class="icon" src="../assets/icon-instagram.svg" alt="face">
        <img class="icon" src="../assets/icon-facebook.svg" alt="insta"/>
        <img class="icon" src="../assets/icon-twitter.svg" alt="pinterest"/>
        <img class="icon" src="../assets/icon-pinterest.svg" alt="twitter"/>
      </div>
    </div>
  </template>
  
  <script>
  export default {
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  .footer{
    padding: 40px 150px;
    background: #232027;
    display: flex;
    justify-content: space-between;
    color: #fff;
  }
  .links{
    display: flex;
  }
  .logo{
  font-size: 24px;
  font-weight: 700;
  cursor: pointer;
  }
  .link{
    margin-left:100px;
    display: flex;
    flex-direction: column;
  }
  .link:first-child{
    margin-left: 0;
  }
  .title{
    margin-bottom: 15px;
    font-weight: 600;
  }
  ul{
    list-style-type: none;
  }
  li{
    cursor: pointer;
    margin-bottom: 5px;
    color: #BDBAC1;
    font-size: 12px;
  }
  .social {
    display: flex;
  }
  .icon{
    width: 20px;
    height: 20px;
    cursor: pointer;
    margin-left: 5px;
  }
  </style>