<template>
  <v-container>
  <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">{{ user.name }}</h3>
            <h3 class="headline mb-0">{{ user.email }}</h3>
            <div></div>
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
