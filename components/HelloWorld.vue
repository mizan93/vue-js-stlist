<template>
  <div class="hello">
   {{msg}}
    <ol>
    
    {{ sayhello(' Morning')}}
    <p>{{owthello}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      msg:'Welcome to vuejs',
    students:['mizan','foyez','imrul','imteaj'],
    fname:'online web',
    lname:'tutor',
    athour_name:'mizan',
    }
  },
  methods:{
    sayhello(dayTime){
      return "Good"+dayTime;
    }
  },
  computed:{
    owthello(){
      return this.fname+' '+this.lname+' given by '+this.athour_name;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
