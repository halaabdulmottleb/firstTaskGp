<template>
  <div class="about">
    <h1>{{pageName}}</h1>
    <p>{{PageDescription}}</p>
  </div>
</template>


<script>
    export default {

        data: function () {

            return {
                pageName: " About US" , 
                PageDescription : "This is description " ,
            };
        }, 

        name : "about"

    };
    
</script>
