<template>

  <v-form ref="form" class="form ma-8">
    <v-row justify="center">
      <v-col cols="8">
        <img src="@/assets/Logo.png" style="background-size: cover;"/>
      </v-col>
    </v-row>
    
    <v-row justify="center">
      <v-col cols="8">
        <v-text-field type="input" label="usuario" 
          hint="Digite o nome de usuário" append-inner-icon="mdi-account-outline"
          v-model="user"
        />
      </v-col>   
    </v-row>
    
    <v-row justify="center">
      <v-col cols="8">
        <v-text-field type="password" label="senha" 
          hint="Digite o sua senha" append-inner-icon="mdi-eye-off-outline"
          v-model="passwd"
        />
      </v-col>
    </v-row>

    <v-row justify="center">
      <v-col cols="8">
        <v-btn style="width: 100%;" id="btn-entrar">Entrar</v-btn>
      </v-col>
    </v-row>
    
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
  .form{
    background-color: #fff;
    max-width: 35%;
    border-radius: 30px;
    min-height: 500px;
  }

  #btn-entrar{
    background-color: #000000;
    color: #fff;
    border-radius: 166px;
  }
</style>