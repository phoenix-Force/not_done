<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
                <h1>Http</h1>
                <div class="form-group">
                  <label for="userName">User Name</label>
                  <input type="text" name="userName" id="userName" v-model = "userName" class="form-control" required>
                </div>
                <div class="form-group">
                  <label for="email">Email</label>
                  <input type="email" name="email" id="email" v-model = "email" class="form-control" required >
                </div>
                <div class="form-group">
                  <button class="btn btn-primary" @click.prevent="submit">Submit</button>
                </div>

            </div>
        </div>
    </div>
</template>



<script>
export default {
  data:()=>{
    return{
      userName:"",
      email:''
    }
  },
  methods:{
    submit(){
      alert(this.userName)
    }

  }
}
</script>

<style lang="scss">

</style>
