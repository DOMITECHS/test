<template>
  <v-app>
    <v-content>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-12">
              <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" sm="8">
                      <v-card-text class="mt-12 " justify="center" >
                        <h1 justify="center" class="text-center display-2 teal--text text--accent-3">Sign in to DOMITECH'S</h1>
                        <div class="text-center mt-4">
                          <v-btn class="mx-2" fab color="black" outlined>
                            <v-icon>fab fa-facebook-f</v-icon>
                          </v-btn>
                          <v-btn class="mr-2" fab color="black" outlined>
                          <v-icon>fab fa-google-plus-g</v-icon>
                          </v-btn>
                          <v-btn class="mr-2" fab color="black" outlined>
                          <v-icon >fab fa-linkedin-in</v-icon>
                          </v-btn>
                        </div>
                        <h4 class="text-center mt-4">Ensure your email for registration</h4>
                        <v-form>
                          <v-text-field 
                          label="Email"
                          name="Email"
                          prepend-icon="email"
                          type="email"
                          color="teal accent-3"></v-text-field>
                          <v-text-field
                          id="password"
                          label="Password"
                          name="password"
                          prepend-icon="lock"
                          type="Password"
                          color="teal accent-3">

                          </v-text-field>
                        </v-form>
                        <h3 class="text-center mt-3">forgot your password</h3>
                      </v-card-text>
                      <div class="text-center mt-1">
                        <v-btn rounded color="teal accent-3" dark>SIGN IN</v-btn>
                      </div>
                    </v-col>
                    <v-col cols="12" md="4" class="teal accent-3">
                      <v-card-text class="white--text mt-12">
                        <h5 class="text-center display-1 ">Hello,Friends!</h5>
                        <h5 class="text-center">Enter your personal details and start your jouney with us</h5>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn rounded outlined="" dark @click="step++">SIGN UP</v-btn>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
                <v-window-item :value="2">
                   <v-col cols="12" md="10">
                      <v-row class="fill height">
                        <v-col cols="12" md="4" class="teal accent-3">
                          <v-card-text class="white--text mt-12">
                        <h5 class="text-center display-1 ">Welcome Back</h5>
                        <h5 class="text-center">Already a member please login width your personal info</h5>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn rounded outlined="" dark @click="step++">SIGN IN</v-btn>
                      </div>
                        </v-col>
                        <v-col cols="12" md="8">
                          <v-card-text class="mt-12">
                            <h5 class="text-center display-1 teal--text text--accent-3">Create Account</h5>
                            <div class="text-center mt-4">
                                <v-btn to="./AboutView" class="mx-2" fab color="black" outlined>
                            <v-icon>fab fa-facebook-f</v-icon>
                          </v-btn>
                          <v-btn class="mr-2" fab color="black" outlined>
                          <v-icon>fab fa-google-plus-g</v-icon>
                          </v-btn>
                          <v-btn class="mr-2" fab color="black" outlined>
                          <v-icon >fab fa-linkedin-in</v-icon>
                          </v-btn>
                            </div>
                            <h4 class="text-center mt-4">Ensure your email for registration</h4>
                             <v-form>
                              <v-text-field
                              label="Name"
                              name="Name"
                              prepend-icon="person"
                              type="text"
                              color="teal accent-3"></v-text-field>
                          <v-text-field 
                          label="Email"
                          name="Email"
                          prepend-icon="email"
                          type="email"
                          color="teal accent-3"></v-text-field>
                          <v-text-field
                          id="password"
                          label="Password"
                          name="password"
                          prepend-icon="lock"
                          type="Password"
                          color="teal accent-3">

                          </v-text-field>
                        </v-form>
                          </v-card-text>
                          <div class="text-center mt-n1">
                            <v-btn rounded color="teal accent-3" dark>SIGN UP</v-btn>
                          </div>
                        </v-col>
                      </v-row>
                    </v-col> 
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>


  export default {
    name: 'HomeView',
  data: () => ({
    step: 1, 
  }),
  groups: {
    source: String
  }
   
  }
</script>
