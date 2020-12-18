<template>
  <div class="home">
      <div class="row">
          <div class="col-md-3">
              <div class="card text-white bg-success mb-3" style="max-width: 18rem; 
                          background: linear-gradient(45deg,#39f 0%,#2982cc 100%)!important;
                         border-color: #2982cc!important;">
                 
                  <div class="card-body">
                      <div class="float-left">
                          <p> 9.823</p> 
                          <p> Members online</p>
                      </div>
                      <div class="float-right">
                          <div class="dropdown">
                              <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                  <img src="https://img.icons8.com/material-outlined/20/000000/settings--v1.png" />
                              </button>
                              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                  <a class="dropdown-item" href="#">Action</a>
                                  <a class="dropdown-item" href="#">Another action</a>
                                  <a class="dropdown-item" href="#">Something else here</a>
                              </div>
                          </div>
                      </div>
                      
                  </div>
              </div>
          </div>

          <div class="col-md-3">
              <div class="card text-white bg-success mb-3" style="max-width: 18rem;
                     background: linear-gradient(45deg,#39f 0%,#2982cc 100%)!important;
                    border-color: #2982cc!important;
                    ">
                  
                  <div class="card-body">
                      <div class="float-left">
                          <p> 9.823</p>
                          <p> Members online</p>
                      </div>
                      <div class="float-right">
                          <div class="dropdown">
                              <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                  <img src="https://img.icons8.com/material-outlined/20/000000/settings--v1.png" />
                              </button>
                              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                  <a class="dropdown-item" href="#">Action</a>
                                  <a class="dropdown-item" href="#">Another action</a>
                                  <a class="dropdown-item" href="#">Something else here</a>
                              </div>
                          </div>
                      </div>

                  </div>
              </div>
          </div>
 
          <div class="col-md-3">
              <div class="card text-white bg-warning mb-3" style="max-width: 18rem;">
                  
                  <div class="card-body">
                      <div class="float-left">
                          <p> 9.823</p>
                          <p> Members online</p>
                      </div>
                      <div class="float-right">
                          <div class="dropdown">
                              <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                  <img src="https://img.icons8.com/material-outlined/20/000000/settings--v1.png" />
                              </button>
                              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                  <a class="dropdown-item" href="#">Action</a>
                                  <a class="dropdown-item" href="#">Another action</a>
                                  <a class="dropdown-item" href="#">Something else here</a>
                              </div>
                          </div>
                      </div>

                  </div>
              </div>
          </div>
          <div class="col-md-3">
              <div class="card text-white bg-success mb-3" style="max-width: 18rem; 
                    background: linear-gradient(45deg,#e55353 0%,#d93737 100%)!important;
                    border-color: #d93737!important;
                    ">
                  
                  
                  <div class="card-body">
                      <div class="float-left">
                          <p> 9.823</p>
                          <p> Members online</p>
                      </div>
                      <div class="float-right">
                          <div class="dropdown">
                              <button class="btn  dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                  <img src="https://img.icons8.com/material-outlined/20/000000/settings--v1.png" />
                              </button>
                              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                  <a class="dropdown-item" href="#">Action</a>
                                  <a class="dropdown-item" href="#">Another action</a>
                                  <a class="dropdown-item" href="#">Something else here</a>
                              </div>
                          </div>
                      </div>

                  </div>
              </div>
          </div>


      </div>
      <div class="row">
          <div class="col-md-12">
              <div class="card" >
                  <div class="card-body">
                      <table class="table table-hover mt-4 table-bordered">
                          <thead class="thead-dark">
                              <tr>
                                  <th scope="col">#</th>
                                  <th scope="col">User</th>
                                  <th scope="col">Email</th>
                                  <th scope="col">Country</th>
                                
                                  
                              </tr>
                          </thead>
                          <tbody>
                             
                              <tr v-for="user in users" v-bind:key ="user.id">
                                  <th scope="row">{{user.id}}</th>
                                  <td>{{ user.name }}</td>
                                  <td>{{user.email}}</td>
                                  <td>{{user.country}}</td>
                              </tr>
                             

                          </tbody>
                      </table>
                  </div>
              </div>
              


          </div>
      </div>
  </div>
</template>

<script>
    import usersData from "../json/usersData.json";
    export default {
        
        data: function () {
            return {
                pageName: "pagename",
                users: usersData , 
            }
        },
        name: "Home",
        
    };
</script>


