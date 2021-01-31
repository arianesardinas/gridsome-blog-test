<template>
  <Layout>
    <div class="container">
      <div class="row">
        <div class="col-4 col-md-4">
          <p>Using color to add meaning only provides a visual indication, which will not be conveyed to users of assistive technologies – such as screen readers. Ensure that information denoted by the color is either obvious from the content itself (e.g. the visible text), or is included through alternative means, such as additional text hidden with the </p>
          <g-link class="nav-link " to="/blog/"><button type="button" class="btn btn-primary">Zum blog</button></g-link>
        </div>
        <div class="col-6 col-md-4">
          <img class="w-full md:w-5/5 z-50" src="../../static/images/undraw_sentiment_analysis_jp6w.svg">
        </div>

      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
