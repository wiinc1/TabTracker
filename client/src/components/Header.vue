<template>
    <v-toolbar fixed class="grey darken-3">
        <v-toolbar-title class="mr-4">
            <span
              class="home"
              @click="navigateTo({name: 'root'})">
              @ the mat
            </span>
        </v-toolbar-title>
        
        <!--<v-toolbar-items>
            <v-btn flat>
                Browse
            </v-btn>
        </v-toolbar-items> -->

        <v-spacer></v-spacer>

        <v-toolbar-items>
            <v-btn flat    
                @click="navigateTo({name: 'login'})">
                Login
            </v-btn>
        </v-toolbar-items>

        <v-toolbar-items>
            <v-btn flat    
                @click="navigateTo({name: 'register'})">
                Sign Up
            </v-btn>
        </v-toolbar-items>
    </v-toolbar> 
</template>

<script>
export default {
  methods: {
    navigateTo (route) {
      this.$router.push(route)
    }
  }
}

</script>

<style scoped>
.home {
    cursor: pointer;
}

.home:hover {
    color: #E9E
}
</style>
