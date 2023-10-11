<template>
    <div>HelloWord</div>
    <h3>Kinolar soni: {{ allSoni }}</h3>
    <h3>Ko'rilgan Kinolar soni: {{ KorilganSoni }}</h3>
</template>
<script>
export default {
    props:{
        allSoni:{
            type: Number,
            required:true
        },
        KorilganSoni:{
            type:Number,
            required:true
        }
    }
}
</script>
<style></style>