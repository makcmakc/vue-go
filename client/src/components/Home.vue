<template>
  <b-jumbotron bg-variant="primary" text-variant="white" border-variant="dark">
    <template slot="header">
      Go &amp; Vue.js App
    </template>
    <template slot="lead">
      This is a simple web application with a Go server/backend and a Vue.js client/frontend.
    </template>
    <hr class="my-4">
    <p>
      <a href="https://golang.org/" target="_blank"><img src="../assets/go.svg" style="height:80px"/></a>
        <img src="../assets/plus.svg" style="height:25px"/>
      <a href="https://vuejs.org/" target="_blank"><img src="../assets/logo.png" style="height:80px"/></a>
        <img src="../assets/equal.svg" style="height:25px"/>
        <img src="../assets/heart.svg" style="height:70px;"/>
    </p>

  </b-jumbotron>
</template>


<style scoped>
  img {
    margin-left: 12px;
  }
</style>