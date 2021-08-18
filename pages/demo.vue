<template>
  <section class="container">
    <div class="view-title">
      demo
      <nuxt-link v-for="item in id_list" :key="item" :to="`/demo/detail/${item}`">
        {{ item }}
      </nuxt-link>
    </div>
    <div class="view">
      <nuxt-child />
    </div>
  </section>
</template>

<script>

export default {
  components: {},
  data () {
    return {
      id_list: ['1', '2', '3', '4']
    }
  }
}
</script>

<style >
.container {
  min-height: 100vh;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
.view{
  width: 100%;
  height: 200px;
  background-color: seagreen;
}
.view-title > a{
  padding: 0 10px;
  margin: 0 5px;
  background-color: salmon;
}
</style>
