<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button @click="GetId">欢迎用户{{PassId}}</button>
  </div>
</template>

<script>
  export default {
    name: "GuestPersonal",
    data() {
      return {
        msg:"顾客个人页面",
        PassId:this.$route.params.UserId,
      }
    },
    methods :{
      GetId (){
        console.log(this.PassId)
      }
    }
  }


</script>

<style scoped>
  h1, h2 {
    font-weight: normal;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
</style>
