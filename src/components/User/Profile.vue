<template>
  <v-container>
  <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-card-title primary-title>
          <div class="text-md-center">
            <h2>Login Success</h2>
            <h4 class="headline mb-0">{{ user.name }}</h4>
            <h4 class="headline mb-0">{{ user.email }}</h4>
          </div>
        </v-card-title>
      </v-card>
    </v-flex>
  </v-layout>
  </v-container>
</template>

<script>
  export default {
    computed: {
      user () {
        return this.$store.getters.user
      }
    }
  }
</script>
