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

</v-col>

</v-row>
</v-container>
</template>

<script>
export default {
data: () => ({

items:[
{ title: 'Alif', link: 'https://www.youtube.com/embed/' + 'EqAM6syuiNs' },
{ title: 'Bay', link: 'https://www.youtube.com/embed/' + '1eYoStEPUNY' },
{ title: 'pay', link: 'https://www.youtube.com/embed/' + 'Sp6zH9Hy8uk' },
{ title: 'Tay', link: 'https://www.youtube.com/embed/' + 'L2zvCcwiGCA' },
{ title: 'Ttay', link: 'https://www.youtube.com/embed/' + 'IGohKIaZkqY' },
{ title: 'Say', link: 'https://www.youtube.com/embed/' + 'mJBAj2sbnos' },
{ title: 'Geem', link: 'https://www.youtube.com/embed/' + 'w3tuCU0ZmKY' },
{ title: 'Chay', link: 'https://www.youtube.com/embed/' + 'DDBKwlatiZE' },
{ title: 'Hay', link: 'https://www.youtube.com/embed/' + 'DchITM2u6To' }, 
{ title: 'Khay', link: 'https://www.youtube.com/embed/' + 'Cpw4vdNi_uw' },
{ title: 'Daal', link: 'https://www.youtube.com/embed/' + 'Nf3kNvmPbpU' },
{ title: 'Ddaal', link: 'https://www.youtube.com/embed/' + 'vGU_JaNdELo' },
{ title: 'Zaal', link: 'https://www.youtube.com/embed/' + 'xWMdZ3xfrpU' },
{ title: 'Ray', link: 'https://www.youtube.com/embed/' + 'kyMKtomXHFc' },
{ title: 'Rray', link: 'https://www.youtube.com/embed/' + '1cq8QYOvN4o' },
{ title: 'Zay', link: 'https://www.youtube.com/embed/' + 'a12e2P7XQ00' }, 
{ title: 'Zhay', link: 'https://www.youtube.com/embed/' + 'ZyokDjbSq7s' },
{ title: 'Seen', link: 'https://www.youtube.com/embed/' + 'V-9NXQK6Neg' },
{ title: 'Sheen', link: 'https://www.youtube.com/embed/' + 'xE-V_0fkNRI' }, 

{ title: 'Suad', link: 'https://www.youtube.com/embed/' + '2NzIt9TZBj8' }, 
{ title: 'Zuad', link: 'https://www.youtube.com/embed/' + 'V1Y74xnB_vQ' }, 

{ title: 'Toay', link: 'https://www.youtube.com/embed/' + 'rvwWIU95DuY' }, 
{ title: 'Zoay', link: 'https://www.youtube.com/embed/' + 'cxCycFCAWuo' }, 

{ title: 'Ain', link: 'https://www.youtube.com/embed/' + 'PufkgYJNv8c' }, 
{ title: 'Ghain', link: 'https://www.youtube.com/embed/' + 'iMt9iL0PetE' }, 

{ title: 'Fay', link: 'https://www.youtube.com/embed/' + 'y3aiOVBIDuU' }, 
{ title: 'Qaaf', link: 'https://www.youtube.com/embed/' + 'vHZSioMOGgE' }, 
{ title: 'Kaaf', link: 'https://www.youtube.com/embed/' + 'Myixy6Pu498' }, 

{ title: 'Gaaf', link: 'https://www.youtube.com/embed/' + 'Z7ldV3v69Uc' }, 
{ title: 'Laam', link: 'https://www.youtube.com/embed/' + 'RIbUu-CCNgk' }, 
{ title: 'Meem', link: 'https://www.youtube.com/embed/' + 'swikgEdepCs' }, 
{ title: 'Noon', link: 'https://www.youtube.com/embed/' + '2FV9liJ1OWM' }, 

{ title: 'Wao', link: 'https://www.youtube.com/embed/' + 'u0xplGmeZHY' }, 
{ title: 'Noon', link: 'https://www.youtube.com/embed/' + '2FV9liJ1OWM' }, 
{ title: 'Do chasmi hay', link: 'https://www.youtube.com/embed/' + 'ResQPrKEDtI' }, 
{ title: 'Noon', link: 'https://www.youtube.com/embed/' + '2FV9liJ1OWM' }, 







],


}),
}
</script>