<template>
  <div>
    <h1>Aplikasi vue.js Gue</h1>
    <my-component nama="Muharafi" umur="19"></my-component>
    
  </div>
</template>

<script>
import MyComponent from './MyComponent.vue';

export default{
  components:{
    MyComponent
  }
}
</script>


