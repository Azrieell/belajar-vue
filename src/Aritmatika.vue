<template>
  <div class="aritmatika">
    <table class="a">
      <tr>
        <td>Angka Ke 1</td>
        <td>: {{ a }}</td>
      </tr>
      <tr>
        <td>Angka Ke 2</td>
        <td>: {{ b }}</td>
      </tr>
      <tr>
        <td>Hasil</td>
        <td>: {{ hasil }}</td>
      </tr>
    </table>
</div>
</template>

<script>
  export default{
    props: ['a','b'],

    data(){
      return{
        angka1: this.a,
        angka2: this.b,
        hasil : parseInt(this.a) + parseInt(this.b),
      }
    }
  };
</script>
