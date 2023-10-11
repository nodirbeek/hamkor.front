<template lang="">
    <div>
        <ul>
            <MoveListItem v-for="movie in movies" :movie="movie"/>
        </ul>
    </div>
</template>
<script>
import MoveListItem from '../move-list-item/MoveListItem.vue';
export default {
    components:{
        MoveListItem,
    },
    props:{
        movies: {
            type: Array,
            required: true
        }
    }
 
}
</script>
<style lang="">
    
</style>