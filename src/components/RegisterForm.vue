<template>
  <div class="register-form">
    <TextBlock title="Create an account" subtitle="Let's get started!"/>
    <div class="register-form__form">
      <InputText label="Name"/>
      <InputText label="Email"/>
      <InputText label="Password"/>
      <InputText label="Confirm password"/>
    </div>
    <div class="buttons">
      <ButtonComponent title="Create Account" color="#FFFFFF" background="#000000" :clickEvent="createAccount" />
      <ButtonComponent title="Sign Up with Google" :clickEvent="signWithGoogle">
        <GoogleIcon/>
      </ButtonComponent>
    </div>
  </div>
</template>

<script>
import TextBlock from "@/components/TextBlock";
import InputText from "@/components/Input";
import ButtonComponent from "@/components/Button";
import GoogleIcon from "@/components/GoogleIcon";


export default {
  name: "RegisterForm",
  components: {GoogleIcon, ButtonComponent, InputText, TextBlock},
  methods: {
    createAccount() {
      alert('Created!')
    },
    signWithGoogle() {
      alert('Signed with Google!')
    }
  }
}
</script>

<style lang="scss" scoped>
.register-form {
  max-width: 500px;
  margin: 0 auto;
  &__form {
    margin: 40px 0 60px;
  }
}
.buttons {
  display: flex;
  flex-direction: column;
  align-items: center;
  row-gap: 20px;
}
</style>