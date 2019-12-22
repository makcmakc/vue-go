<template>
  <div class="card">
    <div class="card-header bg-success h3">
      <fa icon="info-circle" />&nbsp; About
    </div>
    <div class="card-body">
      Developed by Maximillian, 2019/2020<br/>
      Version: {{ version }} <br>
      GitHub: {{ github }}
    </div>
  </div>
</template>


<script>
const packageJson = require ('../../package.json')

export default {
  data: function() {
    return {
      version: packageJson.version,
      github: packageJson.github
    }
  }
}
</script>


