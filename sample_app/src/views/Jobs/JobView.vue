<template>
  <div>
    <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.Id" class="job">
    <router-link :to="{name:'jobdetail',params:{id:job.Id}}">
       <h2>{{job.Title}}</h2>
    </router-link>
  </div>
</div>

</template>

<script>
export default {
data(){
    return{
        jobs:[
            {Title:"Lorem Epsum",Id:1,Detail:"Lorem epsum"},
            {Title:"Lorem Epsum",Id:2,Detail:"Lorem epsum"},
            {Title:"Lorem Epsum",Id:3,Detail:"Lorem epsum"},
            {Title:"Lorem Epsum",Id:4,Detail:"Lorem epsum"}

        ]
    }
}
}
</script>

<style>
.job h2 {
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
}
.job h2:hover {
    background: #ddd;
}
.job a {
    text-decoration: none;
}

</style>