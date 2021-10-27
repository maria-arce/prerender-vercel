<template>
  <teleport to="head">
    <social-meta-tags
    v-for="article in articleFilter" :key="article.id"
      :pageDescription="article.description"
      :Title="article.title"
      :socialImg="article.urlImg"
    >
    </social-meta-tags>
  </teleport>

<div v-for="article in articleFilter" :key="article.id">
<h2>{{article.title}}</h2>
{{article.description}}<br>
<img :src="article.urlImg" />
</div>
    
</template>
<script>
import socialMetaTags from "../components/socialMetaTags.vue"

export default {
  components:{
    socialMetaTags
  },
data(){
return{
    articles:[
        {
        id: 'one',
        title:'First article',
        description: 'These towers of cosmic dust and gas make up part of the Eagle Nebula. ',
        urlImg: 'https://spaceplace.nasa.gov/nebula/en/nebula1.en.jpg'
        },      
        {
        id: 'two',
        title:'Second article',
        description: 'In this image of the Carina Nebula, you can spot tiny yellow and white dots inside pink dust clouds.',
        urlImg: 'https://spaceplace.nasa.gov/nebula/en/nebula2.en.jpg'
        },
        {
        id: 'three',
        title:'Third article',
        description: 'This image might look like a creepy eyeball, but its actually a nebula! NASAs Spitzer Space Telescope captured this image of the Helix Nebula',
        urlImg: 'https://spaceplace.nasa.gov/nebula/en/nebula3.en.jpg'
        }
    ]
}
},    
computed:{
    articleFilter() {
      return this.articles.filter(
        (a) => a.id == this.$route.params.id
      );
    },
}
}
</script>
