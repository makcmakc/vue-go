<template>
  <div id="app">

    <b-navbar toggleable="md" type="dark" variant="primary">
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-navbar-brand to="/"><img src="./assets/vuejs.svg" height="50px"></b-navbar-brand>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav>
          
          <b-nav-item to="/home"><fa icon="home"/>&nbsp; Home</b-nav-item>
          <b-nav-item to="/info"><fa icon="cogs"/>&nbsp; Sys Info</b-nav-item>
          <b-nav-item to="/monitor"><fa icon="tachometer-alt"/>&nbsp; Monitor</b-nav-item>
          <b-nav-item to="/weather"><fa icon="umbrella"/>&nbsp; Weather</b-nav-item>
          <b-nav-item to="/about"><fa icon="info-circle"/>&nbsp; About</b-nav-item>

        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <br/>

    <b-container>
      <transition name="slidedown">
        <router-view/>
      </transition>
    </b-container>

  </div>
</template>

<style>
  html {
    font-size: 20px;
  } 
  #app, html, body {
    height: 100%;
    background-color: #498C9E;
  }
  .b-navbar-nav {
    color: red;
  }
  .slidedown-enter-active {
    transition: transform 0.4s ease-out;
    transform-origin: top;
  }
  .slidedown-enter {
    transform: scaleY(0);
  }
</style>
