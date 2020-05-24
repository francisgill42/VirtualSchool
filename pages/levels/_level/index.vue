<template>

<v-container>
<v-row>

<v-col
v-for="(item, i) in items"
:key="i"
cols="12"
sm="4"
>
<v-card color="primary" :to="'/levels/'+item.id+'/chapters'" dark>

<div class="d-flex flex-no-wrap justify-space-between">

<div>
<v-card-title class="subheading" v-text="item.subject"></v-card-title>
</div>

</div>
</v-card>
</v-col>

</v-row>

<v-row>
<v-col
cols="12"
sm="4"
>
<Back :destination="'/levels'"/>
</v-col>

</v-row>
</v-container>
</template>

<script>
import Back from '../../../components/Back';

export default {
components : { Back },    
data: () => ({

    id: '',
    
    items: [],

}),
async created(){
        this.id = await this.$route.params.level;

                this.$axios.get('get_data_for_level/'+this.id)
                .then((res) =>{
                this.items = res.data.subjects 
                });





}
}
</script>