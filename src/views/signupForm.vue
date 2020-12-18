<template>
    <div class="signupForm">
        <div class="row">
            <div class="col-md-8 offset-md-2">
                <div class="card">
                    <div class="card-header">
                        SignUp Form
                    </div>
                    <div class="card-body">
                        <form>
                            <div class="form-group">
                                <label for="exampleInputEmail1">Name</label>
                                <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" name="emaill" v-model="userData.email">
                                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
                            </div>
                            <div class="form-group">
                                <label for="exampleInputEmail1">Email </label>
                                <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" name="emaill" v-model="userData.email">
                                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
                            </div>

                            <div class="form-group">
                                <label for="exampleInputPassword1">country</label>
                                <input type="password" class="form-control" id="exampleInputPassword1" name="password" v-model="userData.password">
                            </div>

                            <button type="submit" class="btn btn-primary" @click.stop.prevent="submit()">Submit</button>
                        </form>


                    </div>
                </div>
            </div>

           


        </div>
    </div>



</template>
<script>
    export default {
       data: function() {
        return {
          userData: {
            email: '',
            password: ''
          },
          isSubmitted: false
        }
      },

        methods: {
          submit(){
             //if you want to send any data into server before redirection then you can do it here

            this.isSubmitted = true;
            this.$router.push('/');
          }
        }
      }
</script>