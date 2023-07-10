<template>
    <div>
        <h1>Rap</h1>
        <GroupCard :musicgenre="rap"/>
    </div>
    
</template>


<script>
import {mapState} from 'vuex'
import GroupCard from '@/components/GroupCard.vue';

export default {
    name: 'rap-view',
    // props: {},
    data: function(){
        return {}
    },
    computed: {
        ...mapState(['rap'])
    },
    //methods: {}
    // watch: {},
    components: {
        GroupCard
    },
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
}
</script>

<style>

</style>