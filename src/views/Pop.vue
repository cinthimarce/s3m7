<template>
    <div>
        <h1>Pop</h1>
        <GroupCard :musicgenre="pop"/>
    </div>
    
</template>


<script>
import {mapState} from 'vuex'
import GroupCard from '@/components/GroupCard.vue';

export default {
    name: 'pop-view',
    // props: {},
    data: function(){
        return {}
    },
    computed: {
        ...mapState(['pop'])
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