<template>
  <h1>
    Job detail Page
    <p>THe job id is {{id}}</p>
  </h1>
</template>

<script>
export default {
data(){
    return{
        id:this.$route.params.id
    }
}
}
</script>

<style>

</style>