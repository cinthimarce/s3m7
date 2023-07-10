<template>
    <div>
        <h1>Rock</h1>
        <GroupCard :musicgenre="rock"/>
    </div>
    
</template>


<script>
import {mapState} from 'vuex'
import GroupCard from '@/components/GroupCard.vue';

export default {
    name: 'rock-view',
    // props: {},
    data: function(){
        return {}
    },
    computed: {
        ...mapState(['rock'])
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