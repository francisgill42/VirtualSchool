<template>
 
    <v-container>
      <v-row dense>
      
        <v-col
          v-for="(item, i) in items"
          :key="i"
          cols="12"
          sm="4"
        >
          <v-card
            :color="item.color"
            :to="item.link"
            dark
          >
            <div class="d-flex flex-no-wrap justify-space-between">
              <div>
                <v-card-title
                
                  class="headline"
                  v-text="item.title"
                ></v-card-title>

                <!-- <v-card-subtitle v-text="item.link"></v-card-subtitle> -->
              </div>


            </div>
          </v-card>
        </v-col>

              
      </v-row>
    </v-container>
</template>

<script>
  export default {
    auth:false,
    data: () => ({
      
      items:[
        { color: '#385F73',title: 'English', link: '/montessori/english' },
        { color: '#385F73',title: 'Urdu', link: '/montessori/urdu' },
        { color: '#385F73',title: 'Math', link: '/montessori/math' },
        { color: '#385F73',title: 'General Knowledge', link: '/montessori/gk' },
        { color: '#385F73',title: 'Drawing', link: '/montessori/drawing' },
      ],

     
    }),
  }
</script>