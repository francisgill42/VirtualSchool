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
    width="100%"
    :src="item.link" 
    frameborder="0" 
    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>

<v-card-actions class="primary white--text" > {{item.title}} </v-card-actions>

</v-card>

</v-col>

</v-row>
</v-container>
</template>

<script>
export default {
data: () => ({

items:[
{ title: 'Chapter 1', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 2', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 3', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 4', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 5', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 6', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 7', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 8', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 9', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },
{ title: 'Chapter 10', link: 'https://www.youtube.com/embed/' + 'hq3yfQnllfQ' },

],


}),
}
</script>