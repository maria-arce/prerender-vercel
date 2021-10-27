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
        colorName:'Golf Orange',
        colorDescription:'Lorem ipsum dolor sit amet consentur',
        imgSocial:'https://cdn001.wearelean.com/1634819864-718-2g0-social.jpg?auto=compress&q=85&txt-size=20&txt64=RnVlbCBjb25zdW1wdGlvbiBjb21iaW5lZCBpbiBsLzEwMCBrbTogeC54IOKAkyB4LnggKE5FREMpOyB4Lngg4oCTIHgueCAoV0xUUCk7IENPMiBlbWlzc2lvbnMgY29tYmluZWQgaW4gZy9rbTogeHh4IOKAkyB4eHggKE5FREMpOyB4eHgg4oCTIHh4eCAoV0xUUCk=&txt-pad=40&txt-align=bottom,center&txt-color=551d02'
      }
    }

}
</script>

