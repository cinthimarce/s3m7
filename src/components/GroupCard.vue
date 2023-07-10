<template>
    <div class="card_container">
        <div class="card" v-for="album in musicgenre" :key="album.id">
            <h1>{{album.artist}}</h1>
            <img :src="album.image" alt="" width="80%">
            <h2>{{album.album}}</h2>
        </div>
    </div>
        
</template>

<script>
export default {
    name: 'group-card',
    props: {
        musicgenre:{
            type:Array,
            required:true
        }
    },
    data: function(){
        return {}
    },
    // computed: {},
    //methods: {}
    // watch: {},
    // components: {},
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
}
</script>

<style scoped>
.card_container{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        width: 70% ;
        margin:0 auto ;
        gap: 3px;
}
.card{
    padding: 20px;
    border:none;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 6px 12px -2px, rgba(0, 0, 0, 0.3) 0px 3px 7px -3px;
} 
</style>