<template lang="">
    <div>
        <li class="list-group-item" :class="[{like: movie.like}, {favourite: movie.favourite}]"> {{movie.name}}
        <i class="fas fa-star"></i>
        </li>
    </div>

</template>
<script>
export default {
    props:{
        movie:{
            type:Object,
            required:true,
        },
}
}
</script>
<style>
  .list-group-item .fa-star{
    background-color:#eee
  }  
 .list-group-item.like .fa-star{
    background-color:red
  }
</style>