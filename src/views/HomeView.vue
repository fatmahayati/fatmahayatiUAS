<template>
   <h1>Belajar form dan Vue Event</h1>

<div class="container">
 
  <p>Nama</p>
  <input v-model="nama" type="text" class="form-text">
  <p>Nim</p>
  <input v-model="nim" type="text" class="form-text">
  <div class="mt-2">
  <button  type="submit" class="btn btn-info" @click.prevent="simpanData">Simpan</button>
</div>
</div>

<hr>
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
