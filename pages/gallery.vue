<template>
<div class="wrapper">
    <div class="text-container">
        <h1>Gallery</h1>
    </div>
    <div id="gallery-feed">
        <iframe src="//lightwidget.com/widgets/52e13a2a72f4524ca8a661c2a7de45aa.html" scrolling="no" allowtransparency="true" class="lightwidget-widget" style="width:100%;border:0;overflow:hidden;"></iframe>
    </div>
</div>
</template>

<script>
export default {
    head: {
    script: [
      { src: 'https://cdn.lightwidget.com/widgets/lightwidget.js', body: true },
    ]
  }
}
</script>

<style scoped>
#gallery-feed {
    height: 100%;
    overflow: hidden;
}
.text-container {
    padding: 0 0 5%;
}
.text-container h1 {
    text-align: center;
}
</style>
