<template>
  <v-form ref="form" class="ma-10">
    <v-text-field class="field" type="input" label="usuario" 
      hint="Digite o nome de usuário" append-inner-icon="mdi-account-outline"
      v-model="user"
    />

    <v-text-field class="field" type="password" label="senha" 
      hint="Digite o sua senha" append-inner-icon="mdi-eye-off-outline"
      v-model="passwd"
    />

    <v-btn /> 

  </v-form>
  
</template>

<script lang="ts">
  export default{
    data(){
      return{
        user: '',
        passwd: ''
      }
    }
  }
</script>
  

<style>

</style>