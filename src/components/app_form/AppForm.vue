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
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="Hà Nội" v-model="listCheckBox">
                <label class="form-check-label">
                  Hà Nội
                </label>
              </div>
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value=" Đà Nẵng" v-model="listCheckBox">
                <label class="form-check-label" >
                  Đà Nẵng
                </label>
              </div>
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value="HCM" v-model="listCheckBox">
                <label class="form-check-label" >
                  HCM
                </label>
              </div>
              <!-- radio buttom -->
              <div class="form-check">
                <input class="form-check-input" type="radio" name="flexRadioDefault" value="Nam" v-model="radioButton">
                <label class="form-check-label">
                  Nam
                </label>
              </div>
              <div class="form-check">
                <input class="form-check-input" type="radio" name="flexRadioDefault" value="Nữ" v-model="radioButton">
                <label class="form-check-label">
                  Nữ
                </label>
              </div>
          </form>
    </section>
</template>
<script>
export default {
    data(){
        return{
            emailAddress: "",
            listCheckBox: [],
            radioButton: "",
        };
    },
    methods:{
        handleSubmit(){
            console.log(this.emailAddress);
            console.log(this.listCheckBox);
            console.log(this.radioButton);
        }
    }
}
</script>
<style lang="">
    
</style>