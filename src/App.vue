<template>
  <div>
    <!-- <h1><u>Anak yang suka jajan</u></h1> -->
    <!-- <my-component nama="Muharafi Dalilah" umur="17" TTL="Jakarta 09-02-2006" Kelamin="Laki-Laki" agama="Islam" Alamat="Gg.Babakan TVRI No 29"></my-component> -->
    <!-- <Hobi hobi="Main Game"></Hobi> -->
    <!-- <aritmatika a="2" b="8"></aritmatika> -->
    <!-- <latihan nama="Beliau" harga="5000" jumlah="5" uang="100000"></latihan> -->

    <!-- <button @click="setnama()">Set Nama</button>
    <h2>Nama Saya adalah {{ nama }}</h2> -->
  </div>

  <CekUmurComponent nama="Muharafi Dalilah" umur="10"></CekUmurComponent>
</template>

<script>
import MyComponent from './MyComponent.vue';
import Hobi from './Hobi.Vue';
import Aritmatika from './aritmatika.vue';
import Latihan from './Latihan.vue';
import CekUmurComponent from './CekUmurCompnent.vue'

export default{
  components:{
    MyComponent,
    Hobi,
    Aritmatika,
    Latihan,
    CekUmurComponent
  },
  // data(){
  //   return{
  //     nama: ''
  //   }
  // },
  // methods: { 
  //   setnama(){
  //     this.nama = this.nama? '':"Muharafi";
  //   }
  // }
  
}
</script>


