<template>

<v-container>
<v-row>

<v-col
v-for="(item, i) in items"
:key="i"
cols="12"
sm="4"
>
<v-card color="primary" :to="'/levels/'+item.id" dark>

<div class="d-flex flex-no-wrap justify-space-between">

<div>
<v-card-title class="subheading" v-text="item.level"></v-card-title>
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
<Back :destination="'/'"/>
</v-col>

</v-row>
</v-container>
</template>

<script>
import Back from '../../components/Back';

export default {
components : { Back },    
data: () => ({

items: [],

}),
async created(){

const levels = await this.$axios.get('levels');
this.items = levels.data;

}
}
</script>