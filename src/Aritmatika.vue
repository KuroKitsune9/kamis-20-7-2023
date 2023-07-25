<script>
    export default{
        props: ['a', 'b'],

        data() {
            return{
                angka1: this.a,
                angka2: this.b,
                hasil: parseInt(this.a) + parseInt(this.b)
            }
        }


    };
</script>

<template>
<div>
    <p>angka1: {{ a }}</p>
    <p>angka2: {{ b }}</p>
    <p>Hasilnya: {{ hasil }}</p>
</div>
</template>