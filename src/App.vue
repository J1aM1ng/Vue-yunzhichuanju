<template>
  <div id="app">
    <div id="nav">
      <img alt="logo"
           src="./assets/logo.png"
           id="logo">
      <div id="rtr">
        <router-link to="/">首页</router-link>
        <router-link to="/message">产品介绍</router-link>
        <router-link to="/entry">行业解决方案</router-link>
        <router-link to="/zone">应用场景</router-link>
        <router-link to="/about">合作伙伴</router-link>
      </div>

    </div>
    <router-view />
  </div>
</template>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  min-height: 100px;
  padding: 30px;
  margin: 30px;
  margin-bottom: 80px;
  a {
    font-weight: bold;
    color: #1d5d9c;

    &.router-link-exact-active {
      color: #12da76;
    }
  }
  position: relative;
}

#logo {
  width: 150px;
  height: 150px;
  position: absolute;
  left: 20%;
  top: 30%;
  transform: translate(-50%, -50%);
  margin-top: 50px;
}

#rtr {
  position: absolute;
  left: 65%;
  top: 50%;
  transform: translate(-50%, -50%);
}

a {
  text-decoration: none;
  margin: 15px;
}
</style>
