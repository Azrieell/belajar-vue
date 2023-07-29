<template>
  <div>
    <h1 v-if="umur > 17">Selamat Menjelang Dewasa {{ nama }} dengan {{ umur }}</h1>
    <div v-else>
      <button @click="tambahUmur">Tambah Umur</button>
      <h2>Kamu Masih Kecil {{ umur }} Tahun</h2>
    </div>

  </div>
</template>

<script>
  export default {
    props: ['nama', 'umur'],
    data(){
      return{
        umur : this.umur
      }
    },
    methods: {
      tambahUmur() {
        this.umur +=10
      }
    }
  }
</script>