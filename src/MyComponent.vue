<template>
    <div>
        <h2>Halo, {{ nama }}!</h2>
        <P>Umur Kamu: {{ umur }}</P>

        <h2 v-if="umur >= 18">Selamat datang, {{ nama }}!</h2>
        <p v-else>Maaf, kamu belum cukup umur.</p>

        <ul>
            <li v-for="item in items" :key="item.id">{{ item.hobi }}</li>
        </ul>
    </div>    
</template>

<script>
export default {
    props: ['nama', 'umur'], //definisi props "nama dan umur"
data() {
    return {
    items: [
        { id : 1, hobi: "Mmebaca"},
        { id : 2, hobi: "Bermain Game"},
        { id : 3, hobi: "Jalan Jalan"}
    ],
    pesan: 'Halo, ' + this.nama + '!',
    }
}
}
</script>



