<template>
  <v-layout
    column
    justify-center
  >
    <v-flex
      xs12
      sm8
      md9
    >
    
      <v-card  flat>
      
        <v-card-text>
          <p class="subheading">
            Virtual School is the initiative for the schooling system. the purpose of this to help the community
            in pendamic situations due to CRONA VIRUS.  
          </p>
          <div class="text-xs-right">
            <em>
              &mdash; Francis Gill
            </em>
          </div>
          <hr class="my-3">
          &mdash; <a href="/classes">Classes</a>
          <br>
           <hr class="my-3">
          &mdash; <a href = "mailto: francisgill1000@gmail.com">Send Email</a>

        </v-card-text>
      
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
