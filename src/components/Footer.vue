<template>
    <v-footer
    
    padless
     absolute
  >
    <v-card
      flat
      tile
      width="100%"
      class="primary lighten-1 white--text text-center"
    >
      <v-card-text>
        <v-btn
          v-for="i in icons"
          :key="i.url"
          class="mx-4 white--text"
          icon
          target="_blank"
          :href="i.url"
        >
          <v-icon size="24px">
            {{ i.icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="white--text pt-0">
        
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        <strong>Set realistic goals, keep re-evaluating, and be consistent.</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    name: 'Header',
      data: () => ({
      icons: [
        {url:'https://twitter.com/Narendra_1508', icon:'mdi-twitter'},
        {url:'https://www.linkedin.com/in/narendra1508/', icon:'mdi-linkedin'},
        {url:'https://github.com/Narendra1508', icon:'mdi-github'},
      ],
    }),
    computed: {
      localAttrs () {
        const attrs = {}

          attrs.absolute = true
         
        return attrs
      },
    },
  }
  
</script>

<style>


</style>
