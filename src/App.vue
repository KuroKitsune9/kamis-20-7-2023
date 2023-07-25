<template>
  <div>
    <h1><u>Data diri</u></h1>
    <my-component nama="Muharafi Dalilah" umur="17" TTL="Jakarta 09-02-2006" Kelamin="Laki-Laki" agama="Islam" Alamat="Gg.Babakan TVRI No 29"></my-component>
    <Hobi hobi="Main Game"></Hobi>
  </div>
</template>

<script>
import MyComponent from './MyComponent.vue';
import Hobi from './Hobi.Vue';

export default{
  components:{
    MyComponent,
    Hobi
  }
}
</script>


