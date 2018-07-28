<template>
  <section class="container">
    <div>
      hello
      <wp />
    </div>
  </section>
</template>

<script>
import wp from '~/lib/wp.js'

export default {
  async asyncData ({ params }) {
    return wp.posts()
  },
  components: {

  }
}
</script>

<style>
.container {
  margin: 1rem auto;
  width: 90%;
  max-width: 900px;
}
</style>
