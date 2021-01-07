<template>
    <div id="gallery-feed">
        <iframe src="//lightwidget.com/widgets/52e13a2a72f4524ca8a661c2a7de45aa.html" scrolling="no" allowtransparency="true" class="lightwidget-widget" style="width:100%;border:0;overflow:hidden;" id="idIframe"></iframe>
    </div>
</template>

<script>
export default {
    head: {
    script: [
      { src: '~/assets/instaScript.js', body: true },
      { src: '~/assets/iframeResizer.js', body: true },
    ]
  }
}
</script>

<style scoped>
#gallery-feed {
    height: 100%;
    overflow: hidden;
}
</style>
