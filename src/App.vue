<template>
  <div id="app">
    <header class="">さかしるさんぽ</header>
    <Map />
    <footer>
      <div class="button left">
        <img src="@/assets/route.svg" class="icon" />街道<small>から探す</small>
      </div>
      <div class="button right">
        <img src="@/assets/torii.svg" class="icon" />スポット<small
          >から探す</small
        >
      </div>
    </footer>
  </div>
</template>

<script>
import Map from "@/components/Map";

export default {
  name: "App",
  components: {
    Map,
  }
};
</script>

<style>
header {
  color: white;
  font-weight: bold;
  height: 30px;
  vertical-align: middle;
  background-color: #13acc2;
}

footer {
  color: #6c6c71;
  height: 60px;
  font-weight: bold;
  background-color: white;
}

small {
  font-weight: normal;
}
img.icon {
  vertical-align: middle;
  height: 32px;
  width: 32px;
  margin-right: 8px;
}

div.button {
  margin: 0px;
  text-align: center;
  vertical-align: middle;
  height: 58px;
  line-height: 58px;
  display: inline-block;
  border-color: #e4e4e4;
  border-style: solid;
}

div.left {
  width: calc(50% - 2px);
  border-width: 1px 1px 1px 0px;
}

div.right {
  width: calc(50% - 1px);
  border-width: 1px 1px 1px 1px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
