<template>
  <div id="app">
    <h3>All Links</h3>
    <ul>
      <li>
        <router-link to="/" tag="a" exact>Hello World Vue.js</router-link>
      </li>
      <li>
        <router-link to="/earth" tag="a" exact>Hello Earth Vue.js</router-link>
      </li>
      <li>
        <router-link to="/earth/moon" tag="a" exact>Hello Moon Vue.js</router-link>
      </li>
      <li>
        <router-link to="/saturn" tag="a" exact>Hello Saturn Vue.js</router-link>
      </li>
      <li>
        <router-link to="/saturn/titan" tag="a" exact>Hello Titan Vue.js</router-link>
      </li>
      <li>
        <router-link to="/saturn/enceladus" tag="a" exact>Hello Enceladus Vue.js</router-link>
      </li>
      <li>
        <router-link to="/elon/SpaceX/Falcon9" tag="a" exact>Hello Faclon 9 Vue.js</router-link>
      </li>
    </ul>
    <router-view/>
    <bread-crumb></bread-crumb>
  </div>
</template>

<script>
import BreadCrumb from '@/components/BreadCrumb'

export default {
  name: "app",
  components: {
    BreadCrumb
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
