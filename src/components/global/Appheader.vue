<template>
  <div class="header">
         <nav class="navbar navbar-expand-lg navbar-light bg-light " >
             <a class="navbar-brand" href="#">Exam Cloud</a>
             <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-          controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
               <span class="navbar-toggler-icon"></span>
             </button>
             
             <div class="collapse navbar-collapse" id="navbarSupportedContent">
                     <ul class="navbar-nav mr-auto">
                         <router-link to="/" tag="li" class="nav-item active">
                             <a class="nav-link" >Home </a>
                         </router-link> 
                         
                        
                         <router-link to="/login" tag="li" class="nav-item ">
                             <a class="nav-link" >Login</a>
                         </router-link> 
                       <router-link to="/signup" tag="li" class="nav-item ">
                             <a class="nav-link" >signup</a>
                         </router-link> 
                     
                     
                     </ul>
                     <ul class="navbar-nav ml-auto">
                         <li class="nav-item active">
                             
                             <button class="btn nav-link  " type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-     haspopup="true" aria-expanded="false">
                                       <img  v-on:click="toggle"  src="https://img.icons8.com/emoji/20/000000/crescent-moon-emoji.png"/>
                             </button>
                         </li>

                         <li class="nav-item active">
                             <div class="dropdown">
                                   <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-     haspopup="true" aria-expanded="false">
                                       <img  src="https://img.icons8.com/android/20/000000/appointment-reminders.png"/>
                                   </button>
                                   <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                       <a class="dropdown-item" href="#">Action</a>
                                       <a class="dropdown-item" href="#">Another action</a>
                                       <a class="dropdown-item" href="#">Something else here</a>
                                   </div>
                             </div>
                             
                         </li>

                         <li class="nav-item active">
                             <div class="dropdown">
                                   <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-     haspopup="true" aria-expanded="false">
                                        <img  src="https://img.icons8.com/fluent/20/26e07f/new-message.png"/>
                                   </button>
                                   <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                       <a class="dropdown-item" href="#">Action</a>
                                       <a class="dropdown-item" href="#">Another action</a>
                                       <a class="dropdown-item" href="#">Something else here</a>
                                   </div>
                             </div>
                             
                         </li>

                         <li class="nav-item active">
                             <div class="dropdown">
                                   <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-     haspopup="true" aria-expanded="false">
                                       <img  src="https://img.icons8.com/material-sharp/24/4a90e2/data-provider.png"/>
                                   </button>
                                   <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                       <a class="dropdown-item" href="#">Action</a>
                                       <a class="dropdown-item" href="#">Another action</a>
                                       <a class="dropdown-item" href="#">Something else here</a>
                                   </div>
                             </div>
                             
                         </li>



                     </ul>
                     
              </div>
         </nav>
  </div>
</template>


<script>
export default {
  name: "Appheader",
  
}

</script>

<style scoped>
   
 </style>
