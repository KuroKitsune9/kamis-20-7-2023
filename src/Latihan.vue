<template>
    <div>
        <P>Pada tanggal 23 juli tahun 2023 ada seorang pemuda bernama {{ nama }} yang ingin membeli makroni seharga {{ harga }}</P>
        <p>Ageng Membeli makroni sebanyak {{ jumlah }}</p>
        <p>Ageng membayar denga uang sebesar {{ uang }}</p>
        <p>totalnya adalah: {{ total }}</p>
        <p>dan kembalian jajan Ageng adalah {{ hasil }}</p>
    </div>
</template>

<script>
    export default{
        props: ['nama','harga', 'jumlah', 'uang',],

        data(){
            return{
                a: this.harga,
                b: this.jumlah,
                c: this.uang,
                total:0,
                hasil:0
                
            }
        },
        created(){
            this.total = parseInt(this.harga) * parseInt(this.jumlah)
            this.hasil = parseInt(this.uang) - parseInt(this.total)
        }
    }
</script>