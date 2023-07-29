<template>

  <div class="table">
    <table class="center">
      <th>
        <h1>Makaroni Basah</h1>
      </th>
      <tr>
        <td>Nama</td>
        <td>: {{ nama }}</td>
      </tr>
      <tr>
        <td>Tanggal Pembelian</td>
        <td>: {{ tglpembelian }}</td>
      </tr>
      <tr>
        <td>Jenis Makanan</td>
        <td>: {{ jenismakanan }}</td>
      </tr>
      <tr>
        <td>Harga Satu Makanan</td>
        <td>: {{ hargasatumakanan }}</td>
      </tr>
      <tr>
        <td>Jumlah Makanan Yang Dibeli</td>
        <td>: {{ jumlahmakananyangdibeli }}</td>
      </tr>
      <tr>
        <td>Total Pembelian</td>
        <td>: {{ totalpembelian }}</td>
      </tr>
      <tr>
        <td>Cash</td>
        <td>: {{ cash }}</td>
      </tr>
      <tr>
        <td>Kembalian</td>
        <td>: {{ pulangan }}</td>
      </tr>
    </table>

    <button @click="setNama">Set Nama</button>
    <h2>Nama Saya Adalah : {{ nama }}</h2>
  </div>

</template>

<script>
  // export default{
  //   props: ['nama', 'tglpembelian', 'jenismakanan', 'hargasatumakanan', 'jumlahmakananyangdibeli', 'totalpembelianmakanan','cash','kembalian'],
  //   data(){
  //     return{
  //     totalpembelian : parseInt(this.jumlahmakananyangdibeli) * parseInt(this.hargasatumakanan),
  //     }
  //   },
  //   created(){
  //     this.pulangan = parseInt(this.cash) - parseInt(this.totalpembelian)
  //   }
  // }
  
  export default{
    data(){
      return{
        nama : null
      }
    },
    methods:{
    setNama(){
      this.nama = "Azriel"
    }
  }
    }
    

</script>