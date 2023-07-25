<template>
    <div>
        <h1 v-if="umur >= 17">Umur kamu adalah {{ umur }} Selamat menjelang Dewasa {{ nama }}</h1>
        <div v-else>
            <button @click="tambahUmur()">tambah umur</button>
            <h2>Kam Masih Bocil Umur Kamu {{ umur }}</h2>
        </div>
    </div>
</template>

<script>
export default {
    props:['nama', 'umur'],
    data(){
        return{
            umur: this.umur
        }
    },
    methods: {
        tambahUmur(){
            this.umur = parseInt(this.umur) + 10
        }
    }
}
</script>