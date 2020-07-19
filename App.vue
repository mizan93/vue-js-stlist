<template>
  <div>
<v-header></v-header> 
<v-content name="sanjay" v-bind:myplaylist="playlists" chanel-name="online web tutor"
v-bind:students="students"
></v-content>
<v-footer></v-footer>
 </div>
</template>
<script>
import Header from './component/Header.vue'
import Footer from './component/footer.vue'
import Content from './component/content.vue'
export default {
components:{
 "v-header":Header,
 'v-footer':Footer,
 'v-content':Content
},
  data(){
      return{
        playlists:[
              {name:"Wordpress Plugin Development",
              githublink:"https://github.com/owthub/wordpress-plugin",
              title:"Wordpress Plugin Development"  },
              {name:"Wordpress Theme Development",
              githublink:"https://github.com/owthub/wordpress-plugin",
              title:"Wordpress Theme Development"  },
              {name:"Vue Js2 Development",
              githublink:"https://github.com/owthub/wordpress-plugin",
              title:"Wordpress Plugin Development"  },
              
              {name:"WP JSON Rest API Development",
              githublink:"https://github.com/owthub/wordpress-plugin",
              title:"WP JSON Rest API Development"  },
          ],
          students:[
            'rahul','mitun','kabir'
          ]
    }
  }
}
</script>
<style >

</style>
