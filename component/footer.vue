<template>
  <div>
     <footer>
            {{footer_content}}
        </footer>
  </div>
</template>
<script>
export default {
  data(){
      return{
          footer_content:'Copyright @Online Web Tutor Developers 2018',
         
    }
  }
}
</script>
<style scoped>
footer{
                background: #3f51b5f2;
                padding: 7px;
                color: white;
                text-align: center;
            }
</style>
