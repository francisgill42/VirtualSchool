<template>

<v-container>
<v-row>

<v-col
v-for="(item, i) in items"
:key="i"
cols="12"
sm="4"
>
<v-card :color="item.color" :to="item.link" dark>

<div class="d-flex flex-no-wrap justify-space-between">

<div>
<v-card-title class="subheading" v-text="item.title"></v-card-title>
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


items: [
{ color: 'primary',title: 'Montessori', link: '/montessori' },
// { color: 'primary',title: 'Nursery', link: '/nursery' },
// { color: 'primary',title: 'KG 1', link: '/kg1' },
// { color: 'primary',title: 'KG 2', link: '/kg2' },
// { color: 'primary',title: 'Class 1', link: '/class1' },
// { color: 'primary',title: 'Class 2', link: '/class2' },
// { color: 'primary',title: 'Class 3', link: '/class3' },
// { color: 'primary',title: 'Class 4', link: '/class4' },
// { color: 'primary',title: 'Class 5', link: '/class5' },
// { color: 'primary',title: 'Class 6', link: '/class6' },
// { color: 'primary',title: 'Class 7', link: '/class7' },
// { color: 'primary',title: 'Class 8', link: '/class8' },
// { color: 'primary',title: 'Class 9', link: '/class9' },
// { color: 'primary',title: 'Class 10', link: '/class10' },

],
}),
}
</script>