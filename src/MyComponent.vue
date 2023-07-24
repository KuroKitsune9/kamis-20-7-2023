<template>
    <div>
        <h2>Nama: {{ nama }}</h2>
        <h3>Umur: {{ umur }}</h3>
        <h3>Tanggal Lahir: {{ TTL }}</h3>
        <h3>Jenis Kelamin: {{ Kelamin }}</h3>
        <h3>Agama: {{ agama }}</h3>
        <h3>Alamat: {{ Alamat }}</h3>

        <h2 v-if="umur >= 17">Selamat datang, {{ nama }}!</h2>
        <p v-else>Maaf, kamu belum cukup umur.</p>

        <ul>
            <li v-for="item in items" :key="item.id">{{ item.hobi }}</li>
        </ul>
    </div>    
</template>

<script>
export default {
    props: ['nama', 'umur', 'TTL', 'Kelamin', 'agama', 'Alamat'], //definisi props "nama dan umur"
data() {
    return {
    items: [        
        { id : 1, hobi: "Membaca"},
        { id : 2, hobi: "Bermain Game"},
        { id : 3, hobi: "Jalan Jalan"}
    ],
    pesan: 'Halo, ' + this.nama + '!',
    }
}
}
</script>



