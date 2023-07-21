<script setup>
import { ref } from 'vue';
let msg = "Hallo Dunia";
let headName ="<h1>Nama Saya Muharafi Dalilah</h1>";
let pesan ="Cilukba!!";
let terlihat = false;
let todos = [
      { teks: 'Belajar JavaScript' },
      { teks: 'Belajar Vue' },
      { teks: 'Buat proyek keren' }
    ];
let number = 3;
let ok = "YES"
// split message
let message = ref("Hai Vue JS");
function balikkanPesan(){
  message.value = message.value.split('').reverse().join('')
}

// input
let pesan2 = ref("Hai Vue")
</script>

<template>
  <div>
    <span>{{ msg }}</span> <br>
    <span style="color: red;">Ini Warna Merah</span><br>
    <span>{{ headName }}</span> <br>
    <button :disabled="isButtonDisabled">Button</button> <br>
    <span :title="pesan">Arahkan Kursor Kesini</span> <br>
    <span v-if="terlihat">Hallo</span>
    <ol>
      <li v-for="todo in todos">
        {{ todo.teks }}
      </li>
    </ol> <br>
    {{ number + 2 }} <br>
    {{ ok ? 'YES' : 'NO' }} <br>
    {{ msg.split('').reverse().join('') }} <br>
    <!-- text live -->
    <p>{{ pesan2 }}</p>
    <input v-model = "pesan2"> <br>
    <!-- reverse message -->
    <p>{{ message }}</p>
    <button v-on:click="balikkanPesan">Coba Klik!!</button>
  </div>
</template>