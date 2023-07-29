<!-- <template>
  <div>

    <h2>Formulir</h2>

    
    <p>Nama Anda : <input v-model="nama"></p>
    <p>Umur Anda :  <input v-model="umur"></p>
    <p>Asal Sekolah : <input v-model="sekolah"></p>

    <p><button v-on:click="kirim">Kirim {{ kirim }}</button></p>

    <p> Nama Anda :  {{ nama }}</p>
    <p> Umur Anda : {{ umur }}</p>
    <p> Asal Sekolah : {{ sekolah }}</p>
  </div>
</template>


<script setup>
  import {ref} from 'vue'
  let nama = ref('');
  let umur = ref('');
  let sekolah = ref('');
  let kirim = ref('');
</script>


<style>
  h2 {
    text-align: center;
  }
  p{
    text-align: center;
  }
</style> -->



<template>
  <div class="satu">
    <!-- <my-component nama="Azriel R Siddiq" tanggallahir="12 Desember 2005" jeniskelamin="Laki-Laki" agama="Islam" alamat="Leuwi Melang"></my-component> -->
    <!-- <hobi hobi="Momotoran"></hobi> -->
    <!-- <aritmatika a="20" b="20"></aritmatika> -->
    <!-- <Latihan nama="Ageng" tglpembelian="23-07-2023" jenismakanan="Makaroni-Basah" hargasatumakanan="5000" jumlahmakananyangdibeli="10" cash="100000" ></Latihan> -->
    <CekUmurComponent nama="Azriel" umur="10"></CekUmurComponent>
  </div>
</template>

<script>
// import MyComponent from './MyComponent.Vue'
// import hobi from './Hobi.vue'
// import Aritmatika from './Aritmatika.vue'
// import Latihan from './Latihan.vue'
import CekUmurComponent from './CekUmurComponent.vue';
export default {
  components: {
    // MyComponent,
    // hobi,
    // Aritmatika,
    // Latihan,
    CekUmurComponent,
  }
};
</script>

<style>
.satu{
  margin-top: 190px;
}
h1 {
  color: blue;
}
table.center{
  margin-left: auto;
  margin-right: auto;
}
.aritmatika ,a{
  margin-left: 500px;
}

</style>
