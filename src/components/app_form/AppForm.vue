<template>
    <section class="container">
        <h1>Form</h1>
        <form @submit.prevent="handleSubmit">
            <div class="mb-3">
              <label for="Email1" class="form-label">Email address</label>
              <input type="email" class="form-control" id="Email" v-model="emailAddress">
            </div>
            <div class="mb-3">
              <label for="Password1" class="form-label">Password</label>
              <input type="password" class="form-control" id="Password">
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
    </section>
</template>
<script>
export default {
    data(){
        return{
            emailAddress: "",
        };
    },
    methods:{
        handleSubmit(){
            console.log(this.emailAddress);
        }
    }
}
</script>
<style lang="">
    
</style>