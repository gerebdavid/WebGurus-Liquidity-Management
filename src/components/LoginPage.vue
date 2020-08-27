<template>
<v-app>


<v-content id="content">

  <v-card width="500px"  class="mx-auto mt-9" >

  <v-card-title> Login </v-card-title>
  <v-card-text>
  <v-text-field label ="username" prepend-icon="mdi-account-circle"/>
  <v-text-field
   label ="password"
   type="showPassword ? 'text' : 'password'"
   prepend-icon="mdi-lock"
   :append-icon=" showPassword ? 'mdi-eye' : 'mdi-eye-off' "
   @click:append = "showPassword = !showPassword "/>
  </v-card-text>

  <v-divider></v-divider>
  <v-card-actions>
  <v-btn color="info">Login</v-btn>
  </v-card-actions>

  </v-card >



</v-content>
</v-app>

</template>
<script>
export default{
data()
  {
    return{
    showPassword:false
    }

  }
}
</script>
<style>
#content{
background-color: #e0f7fa;
}

</style>
