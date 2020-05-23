<template>
 
    <v-container>
      <v-row>
      
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
                
                  class="subheading"
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
        { color: 'primary',title: 'English', link: '/montessori/english' },
        { color: 'primary',title: 'Urdu', link: '/montessori/urdu' },
        { color: 'primary',title: 'Math', link: '/montessori/math' },
        { color: 'primary',title: 'General Knowledge', link: '/montessori/gk' },
        { color: 'primary',title: 'Drawing', link: '/montessori/drawing' },
      ],

     
    }),
    created(){
      //   let payload = {
      //   token: "mGHuIZ4Eb0kqtgABcGMjrQ",
      //   data: {
      //   links: [
      //     "one","two"
      //   ]
      //   }
      //   };




      // const res = this.$axios.post('https://app.fakejson.com/q',payload)
      // .then(r => console.log(r));
      
      
    }
  }
</script>