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
    <h1>This is an about page</h1>
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
        colorName:'This is the title for About Page',
        colorDescription:'Lorem ipsum dolor sit amet consentur',
        imgSocial:'https://cdn001.wearelean.com/1634819864-718-2g0-social.jpg?auto=compress&q=85'
      }
    }

}
</script>

