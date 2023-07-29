<template>
  <div class="table">


    <my-component nama="Azriel R Siddiq" tanggallahir="12 Desember 2005" jeniskelamin="Laki-Laki" agama="Islam"
      alamat="Leuwi Melang"></my-component>
    <table class="center">
    <tr>
      <td>Hobi</td>
      <td>: {{ hobi }}</td>
    </tr>
    </table>
  </div>
</template>

<script>
  import MyComponent from './MyComponent.Vue';
  export default {
    components: {
      MyComponent
    },
    props: ['hobi'],
  };
</script>