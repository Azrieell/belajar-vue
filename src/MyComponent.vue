<!-- <script setup>
  import {
    ref
  } from 'vue'
  let msg = "barcelona 2 - 8 bayern munchen";
  let nama = "<h1>Nama Saya Azriel</h1>";
  let warna = "Ini Warna Biru"
  let melihat = true
  let pesan = "Umur Saya 18 Tahun"
  let ok = "YES";
  let mesagge = ref('Azriel');
  let pesannn = ref('');
  let selected = ref('')
  function balikkanPesan() {
    mesagge.value = mesagge.value.split('').reverse().join('');
  }

  // let pesann = ref{Hai Vue};
</script>

<template>
  <div>
    <span>{{ msg }}</span> <br>
    <span v-html="nama"></span> <br>
    <span style="color: blue;"> {{ warna }}</span>

    <button v-bind:link="dynamiclink"><a
        href="https://vuejs.org/guide/essentials/template-syntax.html#raw-html">Tombol</a></button> <br>

    <span v-if="melihat">Warna Hitam</span>
    <br>
    <span :title="pesan">Nama Saya Azriel</span> <br>

    <input v-model="pesan" placeholder="edit saya">
    <p>Pesan nya adalah : {{ pesan }}</p><br>

    {{ number + 1 }}
    <br>
    {{ ok ? 'YES' : 'NO' }}

    <input v-model="mesagge">
    <p>Nama Anda : {{ mesagge }}</p>

    <p>{{ mesagge }}</p>
    <button v-on:click="balikkanPesan">balikkanPesan</button>
  </div>
  <br>

  <textarea v-model="pesannn" placeholder="Tambahkan pesan"></textarea>
  <br>
  <span>Pesan dari Multiline adalah:  {{ pesannn }}</span><br>  
  <br>

  <select v-model="selected">
  <option disabled value="">Please select one</option>
  <option>A</option>
  <option>B</option>
  <option>C</option>
</select>
<span>Yang dipilih : {{ selected }}</span>

</template> -->


<template>
  <!-- <div>
    <h2>Nama : {{ nama }}</h2>
    <h2>Tanggal Lahir : {{ tanggallahir }}</h2>
    <h2>Jenis Kelamin : {{ jeniskelamin }}</h2>
    <h2>Agama : {{ agama }}</h2>
    <h2>Alamat : {{ alamat }}</h2>
    <h2></h2>
  </div>
 -->

  <div class="table">
    <table class="center">
      <th>
        <h1>Data Diri</h1>
      </th>
      <tr>
        <td>Nama</td>
        <td>:{{ nama }}</td>
      </tr>
      <tr>
        <td>Tanggal Lahir</td>
        <td>:{{ tanggallahir }}</td>
      </tr>
      <tr>
        <td>Jenis Kelamin</td>
        <td>:{{ jeniskelamin }}</td>
      </tr>
      <tr>
        <td>Agama</td>
        <td>:{{ agama }}</td>
      </tr>
      <tr>
        <td>Alamat</td>
        <td>:{{ alamat }}</td>
      </tr>
      <tr>
        <td>{{ pesan }}</td>
      </tr>
      <tr>
        <td>{{ pesan2 }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
  export default {
    props: ['nama', 'tanggallahir', 'jeniskelamin', 'agama', 'alamat'],

    data(){
      return{
        pesan: 'Halo nama saya : ' + this.nama,
        pesan2 : 'Tanggal Lahir Saya : ' + this.tanggallahir,
      }
    }
  }
</script>