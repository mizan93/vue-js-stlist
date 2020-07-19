<template>
  <div>
     <header>
            <h2>{{ header_msg }}</h2>
            <p>{{header_url}}</p>
        </header>
  </div>
</template>
<script>
export default {
  data(){
      return{
          header_msg:'Welcome to Online Web Tutor Youtube Channel',
          header_url:'http://onlinewebtutorhub.blogspot.in/'
    }
  }
}
</script>
<style scoped>
header{
                background: #3f51b5f2;
                color: white;
                padding: 3px;
                text-align: center;
            }
</style>
