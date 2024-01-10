<template>
   <v-container>
      <v-row align="center" justify="center" >
          <v-col cols="12" sm="10">
            <v-card class="elevation-6 mt-10"  >
             <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h4
                          class="text-center"
                        >Faça login na sua conta</h4>
                        <h6
                          class="text-center  grey--text "
                        >Faça login em sua conta para continuar construindo e <br>editando seus fluxos de integração</h6>
                        <v-row align="center" justify="center">
                          <v-col cols="12" sm="8">
                           
                          <v-text-field
                            label="Email"
                            outlined
                            dense
                            color="green"
                            autocomplete="false"
                           class="mt-16"
                          />
                          <v-text-field
                            label="Senha"
                            outlined
                            dense
                            color="green"
                          autocomplete="false"
                           type="password"
                          
                          />
                            <v-row>
                              <v-col cols="12" sm="7">
                                <v-checkbox
                       
                        label="Lembre de mim"
                        class="mt-n1"
                        color="green"
                      > </v-checkbox>
                              </v-col>
                              <v-col cols="12" sm="5">
                                <span class="caption green--text">Esqueci a senha</span>
                              </v-col>
                            </v-row>
                          <v-btn color="green" dark block tile>Logar</v-btn>
                     
                         <h5
                          class="text-center  grey--text mt-4 mb-3"
                        >Conectar-se usando</h5>
                         <div class="d-flex  justify-space-between align-center mx-10 mb-16">
                        <v-btn depressed outlined color="grey">
                          <v-icon color="red">fab fa-google</v-icon>
                        </v-btn>
                        <v-btn depressed outlined color="grey">
                          <v-icon color="green">fab fa-facebook-f</v-icon>
                        </v-btn>
                        <v-btn depressed outlined color="grey">
                          <v-icon color="light-green lighten-3">fab fa-twitter</v-icon>
                        </v-btn>
                         </div>
                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                    <v-col cols="12" md="6" class="green rounded-bl-xl" >
                    <div style="  text-align: center; padding: 180px 0;">
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Ainda não tem uma conta?</h3>
                        <h6
                          class="text-center"
                        >Vamos configurar tudo para que você possa <br>começar a criar sua primeira experiência de integração.</h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step++">Cadastre-se</v-btn>
                      </div>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
                <v-window-item :value="2">
                  <v-row >
                    <v-col cols="12" md="6" class="green rounded-br-xl">
                     <div style="  text-align: center; padding: 180px 0;">
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Já se cadastrou?</h3>
                        <h6
                          class="text-center"
                        >Faça login na sua conta para que você possa continuar construindo e <br> editando os seus fluxos de integração.</h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step--">Entrar</v-btn>
                      </div>
                      </div>
                    </v-col>

                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h4
                          class="text-center"
                        >Sign Up for an Account</h4>
                        <h6
                          class="text-center  grey--text "
                        >Let's get you all set up so you can start creatin your <br>
                        first onboarding experiance</h6>
                        <v-row align="center" justify="center">
                          <v-col cols="12" sm="8">
                           <v-row>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="Primeiro nome"
                            outlined
                            dense
                            color="green"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="Sobrenome"
                            outlined
                            dense
                            color="green"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           </v-row>
                          <v-text-field
                            label="Email"
                            outlined
                            dense
                            color="green"
                            autocomplete="false"
                          />
                          <v-text-field
                            label="Senha"
                            outlined
                            dense
                            color="green"
                          autocomplete="false"
                           type="password"
                          
                          />
                            <v-row>
                              <v-col cols="12" sm="7">
                                <v-checkbox
                       
                        label="Aceito todos os termos"
                        class="mt-n1"
                        color="green"
                      > </v-checkbox>
                              </v-col>
                              <v-col cols="12" sm="5">
                                <span class="caption green--text ml-n4">Termos &Condições</span>
                              </v-col>
                            </v-row>
                          <v-btn color="green" dark block tile>Cadastre-se</v-btn>
                     
                         <h5
                          class="text-center  grey--text mt-4 mb-3"
                        >Ou siga usando</h5>
                         <div class="d-flex  justify-space-between align-center mx-10 mb-11">
                        <v-btn depressed outlined color="grey">
                          <v-icon color="red">fab fa-google</v-icon>
                        </v-btn>
                        <v-btn depressed outlined color="grey">
                          <v-icon color="green">fab fa-facebook-f</v-icon>
                        </v-btn>
                        <v-btn depressed outlined color="grey">
                          <v-icon color="light-green lighten-3">fab fa-twitter</v-icon>
                        </v-btn>
                         </div>
                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                  </v-row>
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
  
  export default {
    data: () => ({
      step: 1
    }),
    propos: {
      source: String
    }
  }
</script>
<style scoped>

.v-appication .rounded-bl-xl {
  border-bottom-left-radius: 300px !important;
}
.v-appication .rounded-br-xl {
  border-bottom-right-radius: 300px !important;
}
</style>
