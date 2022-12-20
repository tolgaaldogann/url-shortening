<template>
  <div class="statistics">
    <div class="shorten-link-input">
      <input
        v-model="enteredUrl"
        class="input"
        placeholder="Type a link here..."
        type="text"
      />
      <button @click="getShortenLink" class="btn-shorten">Shorten the link</button>
    </div>
    <div class="text">
      <a :href="shortenLink" target="_blank">{{ shortenLink }}</a>
      <h1 class="title">Advanced Statistics</h1>
      <span class="desc"
        >Track how your links are performing across the web with <br />
        our advanced statistics dashboard.</span
      >
    </div>
    <div class="cards">
      <div class="card">
        <img
          class="icons"
          src="../assets/icon-brand-recognition.svg"
          alt="recognition"
        />
        <h3>Lorem, ipsum.</h3>
        <span
          >Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam
          tempora molestiae quaerat id, nihil mollitia!</span
        >
      </div>
      <div class="card">
        <img
          class="icons"
          src="../assets/icon-detailed-records.svg"
          alt="detailed"
        />
        <h3>Lorem, ipsum.</h3>
        <span
          >Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam
          tempora molestiae quaerat id, nihil mollitia!</span
        >
      </div>
      <div class="card">
        <img
          class="icons"
          src="../assets/icon-fully-customizable.svg"
          alt="customizable"
        />
        <h3>Lorem, ipsum.</h3>
        <span
          >Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam
          tempora molestiae quaerat id, nihil mollitia!</span
        >
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      enteredUrl: "",
      shortenLink: "",
    };
  },
  methods: {
    getShortenLink() {
      axios
        .get(`https://api.shrtco.de/v2/shorten?url=${this.enteredUrl}`)
        .then((response) => {
          this.$data.shortenLink = response.data.result.full_short_link;
        })
        .catch((error) => {
          console.log(error);
        });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.statistics {
  display: flex;
  flex-direction: column;
  padding: 40px 150px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  background: #f0f1f6;
}
.shorten-link-input {
  display: flex;
  justify-content: center;
  position: absolute;
  background: #4b406b;
  padding: 20px;
  top: -45px;
  border-radius: 10px;
}
.input {
  width: 600px;
  height: 25px;
  border-radius: 10px;
  padding: 10px;
  margin-right: 10px;
}
.btn-shorten {
  background: #2bd1d1;
  color: #fff;
  border: none;
  padding: 0 30px;
  border-radius: 20px;
  cursor: pointer;
}
.text {
  text-align: center;
  margin-top: 40px;
}
.link {
  color: black;
  font-size: 20px;
  text-decoration: none;
  padding: 10px;
}
.title {
  margin-bottom: 10px;
}
.desc {
  color: #9b9a9f;
}
.cards {
  display: flex;
  margin-top: 100px;
}
.card {
  padding: 50px 10px;
  width: 300px;
  background: #fff;
  margin: 10px;
  position: relative;
}

.icons {
  background: #3d2f54;
  padding: 20px;
  border-radius: 50%;
  position: absolute;
  left: 20px;
  top: -30%;
}
</style>
