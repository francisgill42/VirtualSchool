<template>

<v-container>
<v-row dense>
<v-col
v-for="(item, i) in items"
:key="i"
cols="12"
sm="4"
>
<v-card>

<iframe 
height="225px"
width="100%"
:src="item.link" 
frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen>
</iframe>

<v-card-actions class="primary white--text" > {{item.title}} </v-card-actions>

</v-card>

<Back :destination="'/montessori'"/>
</v-col>

</v-row>
</v-container>
</template>

<script>
import Back from '../../../components/Back';
export default {
components:{ Back },    
data: () => ({

items:[
{ title: 'Alphabets', link: 'https://www.youtube.com/embed/' + 'KBPAI6qLW5o' },
],


}),
created(){}
}
</script>