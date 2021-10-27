<template>
    <meta
      property="og:title"
      :content="Title"
    />
    <meta
      name="twitter:title"
      :content="Title"
    />
    <meta name="twitter:site"
    content="Paint to sample - Porsche" />
    <meta property="og:type" content="website">
    <meta name="twitter:card"
    content="summary"/>
     <meta name="twitter:creator"
    content=" @Porsche"/>
    <meta
      name="description"
      :content="pageDescription"
    />
    <meta
      property="og:description"
      :content="pageDescription"
    />
    <meta
      name="twitter:description"
      :content="pageDescription"
    />
    <meta
      property="og:image"
      :content="socialImg"
    />
        <meta
      name="twitter:image"
      :content="socialImg + '&txt-size=20'"
    />
    <meta
      property="og:image:width"
      content="1450"
    />
    <meta
      property="og:image:height"
      content="1452"
    />

    
</template>
<script>
export default{
    props:{
        Title:String,
        pageDescription:String,
        socialImg:String
    }

}
</script>


