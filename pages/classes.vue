<template>

<v-container>
<v-row dense>

<v-col
v-for="(item, i) in items0"
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

<v-col
v-for="(item, i) in items"
:key="i"
cols="6"
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
data: () => ({

items0:[
{ color: '#385F73',title: 'Montessori', link: '/montessori' },
// { color: '#385F73',title: 'Nursery', link: '/nursery' },
// { color: '#385F73',title: 'KG 1', link: '/kg1' },
// { color: '#385F73',title: 'KG 2', link: '/kg2' },
],

// items: [
// { color: '#1F7087',title: 'Class 1', link: '/class1' },
// { color: '#1F7087',title: 'Class 2', link: '/class2' },
// { color: '#1F7087',title: 'Class 3', link: '/class3' },
// { color: '#1F7087',title: 'Class 4', link: '/class4' },
// { color: '#1F7087',title: 'Class 5', link: '/class5' },
// { color: '#1F7087',title: 'Class 6', link: '/class6' },
// { color: '#1F7087',title: 'Class 7', link: '/class7' },
// { color: '#1F7087',title: 'Class 8', link: '/class8' },
// { color: '#1F7087',title: 'Class 9', link: '/class9' },
// { color: '#1F7087',title: 'Class 10', link: '/class10' },

// ],
}),
}
</script>