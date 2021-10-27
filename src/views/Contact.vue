<template>
    {{colorDescription}}
  <teleport to="head">
    <social-meta-tags
      :pageDescription="colorDescription"
      :Title="colorName"
      :socialImg="imgSocial"
    >
    </social-meta-tags>
  </teleport>
  <div class="about">
    <h1>This is an Contact sample page</h1>
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
        colorName:'Contact title',
        colorDescription:'Mero mero, mero mei',
        imgSocial:'https://cdn001.wearelean.com/1634898562-911-3az-social.jpg?auto=compress&q=85'
      }
    }

}
</script>

