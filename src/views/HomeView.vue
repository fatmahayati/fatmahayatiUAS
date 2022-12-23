<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
  <table class="table">
<thead>
  <tr>
    <th>Nama</th>
    <th>Nim</th>
  </tr>
</thead>
<tbody>
  <tr v-for="item in dataMahasiswa">
    <td>{{item.nama}}</td>
    <td>{{item.nim}}</td>
  </tr>
</tbody>
</table>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
