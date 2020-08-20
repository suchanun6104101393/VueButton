<template>
  <div id="app">
    <img alt="Vue logo" src="https://thumbs.gfycat.com/AbandonedSimpleGlassfrog-small.gif" />
    <HelloWorld msg="SUCHANUN WANNAPINYO" />

    <hr />
    <div class="row">
      <div class="col-6">
        <h2>{{ msg }}</h2>
        <img alt="Vue logo" src="./assets/11.jpg" />
        <h1>{{total1}}</h1>
      </div>
      <div class="col-6">
        <h2>{{ msg }}</h2>
        <img alt="Vue logo" src="./assets/22.jpg" />
        <h1>{{total2}}</h1>
      </div>
      <div class="col-6">
        <CsButton @cc="sum" />
      </div>
      <div class="col-6">
        <CsButton @cc="sum1" />
      </div>
      <div class="col-6">
        <h2>{{ msg }}</h2>
        <img alt="Vue logo" src="./assets/33.jpg" />
        <h1>{{total3}}</h1>
      </div>
      <div class="col-6">
        <h2>{{ msg }}</h2>
        <img alt="Vue logo" src="./assets/44.jpg" />
        <h1>{{total4}}</h1>
      </div>

      <div class="col-6">
        <CsButton @cc="sum2" />
      </div>

      <div class="col-6">
        <CsButton @cc="sum3" />
      </div>
    </div>
  </div>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CSButton.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    CsButton,
  },
  data: function () {
    return {
      total1: 0,
      total2: 0,
      total3: 0,
      total4: 0,
    };
  },
  methods: {
    sum(counterValue) {
      this.total1 = counterValue;
    },

    sum1(counterValue) {
      this.total2 = counterValue;
    },
    sum2(counterValue) {
      this.total3 = counterValue;
    },
    sum3(counterValue) {
      this.total4 = counterValue;
    },
  },
};
</script>

<style>
  
#app {
  font-family: "Ultra", serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #800000;
  margin-top: 60px;
  background: url(https://i.pinimg.com/originals/28/ae/0a/28ae0a1deeb7e1b532409e6dc6c7918d.jpg)
    no-repeat center fixed;
  background-size: cover;
}
</style>