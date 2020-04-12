<template>
<div id="app">
  <div class="header">
    <router-link to="/">
      <div class="logo">
        <img src="/rings.png">
      </div>
    </router-link>
    <div class="title">
      <h1>The Wedding Blog</h1>
    </div>
    <div class="nav-link"><router-link to="/post"> New Post</router-link></div>
  </div>
  <div class="content">
    <router-view />
  </div>
  <div class="h-divider"></div>
  <div class="footer">
    <div class="a-link"><router-link to="/post"> New Post</router-link></div>
    <div class="github"><p>Find Kinsley on <a href="https://github.com/kinsleyc/creative-project-4" target="_blank">Github</a></p></div>
  </div>
</div>
</template>

<style>
html {
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  background: #fff;
  padding: 0px;
  margin: 0px;
}

/* Header */
.header {
  display: flex;
  padding: 10px 100px 0px 100px;
  background-color: #ffcce6;
  color: black;
}

.header a {
  text-decoration: none;
  color: black;
}

.header a:hover {
  text-decoration: underline;
}

.logo img {
  width: 100px;
}

.title {
  margin-top: 5px;
}

.title h1 {
  font-size: 40px;
  font-family: 'Snell Roundhand', cursive;
}

.nav-link {
  position: absolute;
  top: 60px;
  right: 50px;
}

.content {
  padding: 20px 100px;
  min-height: 500px;
}

/* Footer */
.footer {
  display: flex;
  flex-direction: column;
  height: 50px;
  padding: 20px 100px 0px 100px;
  background: #e3e3e3;
  font-size: 12px;
  align-items: center;
}

.footer a {
  color: #000;
}

.footer a:hover {
  text-decoration: none;
}

.h-divider {
    height: 1px;
    width: 100%;
    border-top: 1px solid black;
}

h1 {
  font-size: 20px;
}

h2 {
  font-size: 14px;
}
</style>
