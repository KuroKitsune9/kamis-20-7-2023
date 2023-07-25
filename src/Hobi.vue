<template>
    <div>
        <h2>Hobi Saya: {{ hobi }}</h2>

        <!-- <ul>
            <li v-for="item in items" :key="item.id">{{ item.hobi }}</li>
        </ul> -->
    </div>
</template>

<script>
    export default{
        props: ['hobi'],
//         data() {
//     return {
//     items: [        
//         { id : 1, hobi: "Membaca"},
//         { id : 2, hobi: "Bermain Game"},
//         { id : 3, hobi: "Jalan Jalan"}
//     ],
//     pesan: 'Halo, ' + this.nama + '!',
//     }
// }
    }
</script>