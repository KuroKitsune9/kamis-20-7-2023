<template>
    <div>
        <h2>Halo, {{ nama }}!</h2>
        <P>Umur Kamu: {{ umur }}</P>
    </div>    
</template>

<script>
export default{
    props: ['nama', 'umur'], //definisi props "nama dan umur"
}
</script>