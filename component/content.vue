<template>
  <div>
     
        <div id="content">
            <h3>Playlists</h3>
            {{chanelName}}
            <ul>
                <li v-for="playlist in myplaylist" :key="playlist">
                    <a
                     v-bind:href="playlist.githublink"
                     v-bind:title="playlist.title"
                      target="_blank"
                      >{{playlist.name}}</a>
                </li>
            </ul>
            <h2>Student list</h2>
            <ul >
                <li v-for="student in students" :key="student">{{student}}</li>
            </ul>
            {{call()}}
        </div>
  </div>
</template>
<script>
export default {
    //props:['name','myplaylist','chanelName'],
    props:{
        students:{
type:Array
        },
name:{
    type:String,
    required:true
},
myplaylist:{
    type:Array
},
chanelName:{
    type:String
}
    },
  data(){
      return{
          msg:'This is simple msg'
    }},
    methods:{
        call:function(){
console.log(this.name);
        }
    }
  }
</script>
<style scoped>
#content{
              text-align: center;
            }

            #content ul{
                list-style: none;
            }

            #content ul li{
                font-size: 19px;
                padding: 6px;
                color: #38190e;
            }

            #content h3{
                text-align: center;
            }
</style>
